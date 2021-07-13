# Parte 2 Modulo 6

# Exploración de los servicios de Azure Storage

## Aspectos básicos de Disk Storage

Disk Storage proporciona discos para Azure Virtual Machines. Las aplicaciones y otros servicios pueden acceder a estos discos y usarlos cuando sea necesario, igual que se haría en escenarios locales. Disk Storage permite que los datos se almacenen de forma persistente y que se acceda a ellos desde un disco duro virtual conectado.

Los discos tienen diferentes tamaños y niveles de rendimiento, desde unidades de estado sólido (SSD) a unidades de disco duro (HDD) giratorias tradicionales, con diferentes niveles de rendimiento. Puede usar discos SSD y HDD estándar para cargas de trabajo menos críticas, discos SSD Premium para aplicaciones de producción críticas y Ultra Disks para cargas de trabajo con un uso intensivo de datos como SAP HANA, bases de datos de nivel superior y cargas de trabajo con mucha actividad de transacciones. Azure han ofrecido durabilidad de nivel empresarial de forma coherente para los discos de infraestructura como servicio (IaaS), con una tasa de error anualizada del 0 % líder del sector.

## Aspectos básicos de Azure Blob Storage

Azure Blob Storage es una solución de almacenamiento de objetos para la nube. Puede almacenar grandes cantidades de datos, como datos de texto o binarios. Azure Blob Storage es no estructurado, lo que significa que no hay ninguna restricción en cuanto a los tipos de datos que puede contener. Blob Storage puede administrar miles de cargas simultáneas, cantidades enormes de datos de vídeo, archivos de registro en constante crecimiento y es accesible desde cualquier lugar con conexión a Internet.

Los blobs no están limitados a formatos de archivo comunes. Un blob podría contener gigabytes de datos binarios transmitidos desde un instrumento científico, un mensaje cifrado para otra aplicación o datos en un formato personalizado para una aplicación que se está desarrollando. Una ventaja del almacenamiento en blobs con respecto al almacenamiento en disco es que no requiere que los desarrolladores piensen en discos o los administren; los datos se cargan como blobs y Azure se encarga de las necesidades de almacenamiento físico.

## Blob Storage resulta ideal para lo siguiente:

Visualización de imágenes o documentos directamente en un explorador.
Almacenamiento de archivos para acceso distribuido.
Streaming de audio y vídeo.
Almacenamiento de datos para copia de seguridad y restauración, recuperación ante desastres y archivado.
Almacenamiento de datos para el análisis en local o en un servicio hospedado de Azure.
Almacenamiento de hasta 8 TB de datos para máquinas virtuales.
Los blobs se almacenan en contenedores, lo que ayuda a organizar los blobs en función de sus necesidades empresariales.

## Descripción de los niveles de acceso de blobs

Los datos almacenados en la nube pueden crecer a un ritmo exponencial. Para administrar los costos de las crecientes necesidades de almacenamiento, resulta útil organizar los datos en función de atributos como la frecuencia de acceso y el período de retención planeada. Los datos almacenados en la nube pueden ser diferentes según la forma en que se generan, se procesan y se accede a ellos a lo largo de su vigencia. A algunos datos se accede y se modifican activamente a lo largo de su duración. A algunos datos se accede con frecuencia al principio de su duración, mientras que el acceso cae drásticamente a medida que envejecen los datos. Algunos datos permanecen inactivos en la nube y, después de que se almacenan, no se accede a ellos prácticamente nunca. Para dar cabida a estas diferentes necesidades de acceso, Azure proporciona varios niveles de acceso, que puede usar para equilibrar los costos de almacenamiento con sus necesidades de acceso.

Azure Storage ofrece diferentes niveles de acceso para el almacenamiento de blobs, lo que le ayuda a almacenar datos de objetos de la manera más rentable. Entre los niveles de acceso disponibles se incluyen:

* Nivel de acceso frecuente: optimizado para almacenar datos a los que se accede con frecuencia (por ejemplo, imágenes para el sitio web).
* Nivel de acceso esporádico: optimizado para datos a los que se accede con poca frecuencia y que se almacenan al menos durante 30 días (por ejemplo, las facturas de los clientes).
* Nivel de acceso de archivo: conveniente para datos a los que raramente se accede y que se almacenan durante al menos 180 días con requisitos de latencia flexibles (por ejemplo, copias de seguridad a largo plazo).

Las siguientes consideraciones se aplican a los distintos niveles de acceso:

* Solo los niveles de acceso frecuente y esporádico se pueden establecer en el nivel de cuenta. El nivel de acceso de archivo no está disponible en el nivel de cuenta.
Los niveles frecuente, esporádico y de archivo se pueden establecer en el nivel de blob durante la carga o después de esta.
* Los datos del nivel de acceso esporádico pueden tolerar una disponibilidad ligeramente inferior, pero aun así requieren una gran durabilidad, una latencia de recuperación y unas características de rendimiento similares a las de los datos de acceso frecuente. En el caso de los datos de acceso esporádico, un contrato de nivel de servicio (SLA) con una disponibilidad ligeramente inferior y unos costos de acceso mayores, en comparación con los datos de acceso frecuente, es aceptable a cambio de unos costos de almacenamiento menores.
* El almacenamiento de archivo almacena datos sin conexión y ofrece los menores costos de almacenamiento, pero los mayores costos de acceso y rehidratación de datos.

## Aspectos básicos de Azure Files

Azure Files ofrece recursos compartidos de archivos totalmente administrados en la nube a los que se puede acceder mediante los protocolos del Bloque de mensajes del servidor y Network File System (versión preliminar). Los recursos compartidos de Azure se pueden montar simultáneamente en implementaciones de Windows, Linux y macOS en la nube o locales. Las aplicaciones que se ejecutan en máquinas virtuales o servicios en la nube de Azure pueden montar un recurso compartido de almacenamiento de archivos para acceder a datos de archivos, del mismo modo que una aplicación de escritorio montaría un recurso compartido SMB normal. Cualquier número de roles o máquinas virtuales de Azure puede montar y acceder simultáneamente al recurso compartido de almacenamiento de archivos. Los escenarios de uso típicos serían el uso compartido de archivos en cualquier lugar del mundo, los datos de diagnóstico o el uso compartido de datos de aplicación.


### Use Azure Files para las siguientes situaciones:


Muchas aplicaciones locales usan recursos compartidos de archivos. Azure Files facilita la migración de esas aplicaciones que comparten datos a Azure. Si monta el recurso compartido de archivos en la misma letra de unidad que usa la aplicación local, la parte de la aplicación que accede al recurso compartido de archivos debe funcionar con cambios mínimos, si los hay.
Almacene archivos de configuración en un recurso compartido de archivos y acceda a ellos desde varias máquinas virtuales. Las herramientas y utilidades que usen varios desarrolladores de un grupo pueden almacenarse en un recurso compartido de archivos, lo que garantiza que todos los usuarios puedan encontrarlas y que utilizan la misma versión.
Escriba datos en un recurso compartido de archivos y procese o analice los datos más adelante. Por ejemplo, puede que desee hacerlo con registros de diagnóstico, métricas y volcados de memoria.


