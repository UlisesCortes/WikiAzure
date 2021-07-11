# Parte 2 Modulo 4

# Introducción a los servicios de Azure Compute

Azure Compute es un servicio de informática a petición para ejecutar aplicaciones basadas en la nube. Se proporcionan recursos informáticos como discos, procesadores, memoria, redes y sistemas operativos. Los recursos están disponibles a petición y normalmente pueden estar disponibles en minutos o incluso en segundos. Solo se paga por los recursos que se usan y solo durante el tiempo que se usan.

Azure admite una amplia gama de soluciones informáticas para el desarrollo y las pruebas, la ejecución de aplicaciones y la ampliación del centro de datos. El servicio es compatible con Linux, Windows Server, SQL Server, Oracle, IBM y SAP. Azure también tiene muchos servicios que pueden ejecutar máquinas virtuales (VM). Cada servicio proporciona opciones distintas en función de los requisitos. Algunos de los servicios más destacados son los siguientes:

- [Azure Virtual Machines](#Azure-Virtual-Machines) 
- [Azure App Service](#Azure-App-Service) 
- [Azure Container Instances](#Azure-Container-Instances) 
- [Azure Functions (o informática sin servidor)](#Informatica-sin-servidor ) 

# Máquinas virtuales
Las máquinas virtuales son emulaciones de software de equipos físicos. Incluyen un procesador virtual, memoria, almacenamiento y recursos de red. Hospedan un sistema operativo, y se puede instalar y ejecutar software, al igual que en un equipo físico. Al utilizar un cliente de escritorio remoto, puede usar y controlar la máquina virtual como si se estuviera sentado delante de ella.
Gracias a Azure Virtual Machines, puede crear y utilizar máquinas virtuales en la nube. Virtual Machines proporciona infraestructura como servicio (IaaS) y se puede usar de maneras diferentes. Cuando necesite un control total sobre el entorno y el sistema operativo, las máquinas virtuales son la opción idónea. Al igual que sucede en un equipo físico, se puede personalizar todo el software que se ejecuta en la máquina virtual. Esta capacidad resulta útil cuando se ejecuta software personalizado o configuraciones de hospedaje personalizadas.

# Azure Virtual Machines
Gracias a Azure Virtual Machines, puede crear y utilizar máquinas virtuales en la nube. Estas máquinas virtuales proporcionan una infraestructura como servicio (IaaS) en forma de un servidor virtualizado y se pueden usar de muchas formas. Al igual que sucede en un equipo físico, se puede personalizar todo el software que se ejecuta en la máquina virtual. Las máquinas virtuales son una opción ideal cuando se necesita lo siguiente:
- Control total sobre el sistema operativo (SO).
- Capacidad de ejecutar software personalizado.
- Usar configuraciones de hospedaje personalizadas.
Una máquina virtual de Azure le ofrece la flexibilidad de la virtualización sin necesidad de adquirir y mantener el hardware físico que ejecuta la máquina virtual. Todavía se necesita configurar, actualizar y mantener el software que se ejecuta en la máquina virtual.
Al seleccionar una imagen de máquina virtual preconfigurada, podrá crear y aprovisionar una máquina virtual en cuestión de minutos. La selección de una imagen es una de las decisiones más importantes que tomará cuando cree una máquina virtual. Una imagen es una plantilla que se usa para crear una máquina virtual. Estas plantillas ya incluyen un sistema operativo y, a menudo, otro software, como herramientas de desarrollo o entornos de hospedaje web.

## Ejemplos de cuándo usar máquinas virtuales
- **Durante las pruebas y el desarrollo.** Las máquinas virtuales proporcionan una manera rápida y sencilla de crear distintas configuraciones de sistema operativo y de aplicación. El personal encargado de las pruebas y del desarrollo puede eliminar fácilmente las máquinas virtuales cuando ya no las necesite.
- **Al ejecutar aplicaciones en la nube.** La capacidad de ejecutar determinadas aplicaciones en la nube pública, en lugar de crear una infraestructura tradicional para ejecutarlas, puede proporcionar importantes beneficios económicos. Por ejemplo, es posible que una aplicación necesite controlar las fluctuaciones en la demanda. Apagar las máquinas virtuales cuando no las necesite o iniciarlas rápidamente para satisfacer un aumento repentino de la demanda significa que solo paga por los recursos que se usan.
- **A la hora de extender el centro de recursos a la nube.** Una organización puede extender las capacidades de su propia red local mediante la creación de una red virtual en Azure y al agregar máquinas virtuales a esa red virtual. Las aplicaciones como SharePoint se pueden ejecutar en una máquina virtual de Azure en lugar de hacerlo de forma local. Esta disposición hace que sea más sencilla o menos costosa de implementar que en un entorno local.
- **Durante la recuperación ante desastres.** Igual que con la ejecución de ciertos tipos de aplicaciones en la nube y con la ampliación de una red local a la nube, se puede obtener un ahorro considerable en costos mediante el uso de un enfoque basado en IaaS para la recuperación ante desastres. Si se produce un error en un centro de datos principal, puede crear máquinas virtuales que se ejecuten en Azure para ejecutar las aplicaciones críticas y, después, puede apagarlas cuando el centro de datos principal vuelva a estar operativo.

## Traslado a la nube con máquinas virtuales
Las máquinas virtuales también son una opción excelente cuando se mueve de un servidor físico a la nube (también conocido como Lift-and-shift). Puede crear una imagen del servidor físico y hospedarla en una máquina virtual con pocos o ningún cambio. Al igual que un servidor físico local, las máquinas virtuales requieren mantenimiento. Por tanto, debe actualizar el sistema operativo y su software.

## Escalado de máquinas virtuales en Azure
Se pueden ejecutar máquinas virtuales únicas para pruebas, desarrollo o tareas secundarias. También se pueden agrupar las máquinas virtuales para proporcionar alta disponibilidad, escalabilidad y redundancia. Con independencia de cuáles sean los requisitos de tiempo de actividad, Azure cuenta con varias características para que pueda cumplirlos. Estas características son:
- Conjuntos de escalado de máquinas virtuales
- Azure Batch
 
## ¿Qué son los conjuntos de escalado de máquinas virtuales?
Los conjuntos de escalado de máquinas virtuales permiten crear y administrar un grupo de máquinas virtuales idénticas, de carga equilibrada. Imagine que está ejecutando un sitio web que permite a los científicos cargar imágenes de astronomía que deben procesarse. Si ha duplicado la máquina virtual, normalmente necesitará configurar un servicio adicional para enrutar las solicitudes entre varias instancias del sitio web. Los conjuntos de escalado de máquinas virtuales pueden encargarse de ello.

Los conjuntos de escalado le permiten administrar, configurar y actualizar de forma centralizada un gran número de máquinas virtuales en cuestión de minutos para proporcionar aplicaciones altamente disponibles. El número de instancias de máquina virtual puede aumentar o disminuir automáticamente según la demanda, o de acuerdo con una programación definida. Con los conjuntos de escalado de máquinas virtuales, puede crear servicios a gran escala para áreas como proceso, macrodatos y cargas de trabajo de contenedor.

## ¿Qué es Azure Batch?
Azure Batch permite trabajo por lotes paralelos a gran escala y de informática de alto rendimiento (HPC) con la capacidad de escalar a decenas, cientos o miles de máquinas virtuales.

## Cuando esté listo para ejecutar un trabajo, Batch:

- Iniciará un grupo de máquinas virtuales de proceso de forma automática.
- Instalará aplicaciones y datos de almacenamiento provisional.
- Ejecutará trabajos con tantas tareas como tenga.
- Identificará errores.
- Reordenará la cola de trabajo.
- Reducirá verticalmente el grupo a medida que se complete el trabajo.
Puede haber situaciones en las que se necesite potencia informática sin procesar o potencia de cálculo a nivel de superequipo. Azure proporciona estas capacidades


## Conjuntos de escalado de máquinas virtuales
Los conjuntos de escalado de máquinas virtuales son un recurso de Azure Compute que puede usar para implementar y administrar un conjunto de máquinas virtuales idénticas. Con todas las máquinas virtuales configuradas de la misma manera, los conjuntos de escalado de máquinas virtuales están diseñados para admitir el escalado automático verdadero. No es necesario el aprovisionamiento previo de las máquinas virtuales. Por este motivo, es más sencillo compilar servicios a gran escala cuyo destino sean las cargas de trabajo en contenedores, de macroproceso y macrodatos. A medida que la demanda aumente, se pueden agregar más instancias de máquina virtual. A medida que la demanda disminuya, se pueden quitar más instancias de máquina virtual. El proceso puede ser manual, automatizado o una combinación de ambos.

## Containers y Kubernetes
Container Instances y Azure Kubernetes Service son recursos de Azure Compute que puede usar para implementar contenedores y administrarlos. Los contenedores son entornos de aplicación ligeros y virtualizados. Están diseñados para crearse, escalarse horizontalmente y detenerse dinámicamente de forma rápida. Puede ejecutar varias instancias de una aplicación en contenedores en un único equipo host.


# Azure App Service
Con Azure App Service puede compilar, implementar y escalar de forma rápida aplicaciones de API, móviles y web de nivel empresarial que se pueden ejecutar en cualquier plataforma. Puede satisfacer los exigentes requisitos de rendimiento, escalabilidad, seguridad y cumplimiento mientras usa una plataforma totalmente administrada para realizar el mantenimiento de la infraestructura. App Service es una oferta de plataforma como servicio (PaaS).

## Decisión de cuándo usar Azure App Service
App Service permite crear y hospedar aplicaciones web, trabajos en segundo plano, back-ends móviles y API RESTful en el lenguaje de programación que prefiera, sin tener que administrar la infraestructura. Ofrece escalado automático y alta disponibilidad. App Service es compatible con Windows y Linux, y permite implementaciones automatizadas desde GitHub, Azure DevOps o cualquier repositorio Git para admitir un modelo de implementación continua.
Esta entorno de plataforma como servicio (PaaS) permite centrarse en el sitio web y la lógica de la API, mientras que Azure se encarga de la infraestructura para ejecutar y escalar las aplicaciones web.

## Costos de Azure App Service
Se paga por los recursos de Azure Compute que la aplicación usa mientras procesa las solicitudes según el plan de App Service que elija. El plan de App Service determina la cantidad de hardware dedicado al host. Por ejemplo, el plan determina si el hardware es dedicado o compartido y cuánta memoria se le reserva. Incluso hay un nivel gratuito que puede usar para hospedar sitios pequeños y con poco tráfico.

## Tipos de servicios de aplicaciones
Con App Service, puede hospedar la mayoría de los estilos de servicio de aplicación más comunes, como los siguientes:

- [Aplicaciones web](#Aplicaciones-web)
- [Aplicaciones de API](#Aplicaciones-de-API)
- [Trabajos web](#Trabajos-web)
- [Aplicaciones móviles](#Aplicaciones-móviles)
 
App Service controla la mayoría de las decisiones sobre la infraestructura que se tratan en el hospedaje de aplicaciones accesibles desde la web:

- La implementación y administración se integran en la plataforma.
- Los puntos de conexión se pueden proteger.
- Los sitios se pueden escalar rápidamente para controlar cargas de tráfico elevado.
- El equilibrio de carga integrado y el administrador de tráfico proporcionan alta disponibilidad.
Todos estos estilos de aplicación se hospedan en la misma infraestructura y comparten estas ventajas. Esto convierte a App Service en la elección ideal para hospedar aplicaciones orientadas a la web.

### Aplicaciones web
App Service incluye compatibilidad completa para hospedar aplicaciones web mediante ASP.NET, ASP.NET Core, Java, Ruby, Node.js, PHP o Python. Puede elegir Windows o Linux como sistema operativo del host.

### Aplicaciones de API
Al igual que al hospedar un sitio web, puede compilar API web basadas en REST mediante el lenguaje y el marco que prefiera. Se obtiene compatibilidad completa con Swagger y la posibilidad de empaquetar y publicar la API en Azure Marketplace. Las aplicaciones producidas se pueden consumir desde cualquier cliente basado en HTTP o HTTPS.

### Trabajos web
Se puede usar la característica WebJobs para ejecutar un programa (.exe, Java, PHP, Python o Node.js) o un script (.cmd, .bat, PowerShell o Bash) en el mismo contexto que una aplicación web, aplicación de API o aplicación móvil. Los puede programar o ejecutar un desencadenador. Los trabajos web suelen usarse para ejecutar tareas en segundo plano como parte de la lógica de aplicación.

### Aplicaciones móviles
Use la característica Mobile Apps de App Service a fin de compilar rápidamente un back-end para aplicaciones iOS y Android. Con unos pocos clics en Azure Portal, puede realizar lo siguiente:

- Almacenar los datos de aplicaciones móviles en una base de datos SQL basada en la nube.
- Autenticar a clientes con proveedores sociales comunes, como MSA, Google, Twitter y Facebook.
- Enviar notificaciones de inserción.
- Ejecutar lógica de back-end personalizada en C# o Node.js.
En el lado de la aplicación móvil, hay compatibilidad con el SDK para aplicaciones nativas de iOS y Android, Xamarin y React.




# ¿Qué son los contenedores?
Los contenedores son un entorno de virtualización. Al igual que la ejecución de varias máquinas virtuales en un solo host físico, se pueden ejecutar varios contenedores en un solo host físico o virtual. A diferencia de las máquinas virtuales, no se administra el sistema operativo de un contenedor. Las máquinas virtuales parecen ser una instancia de un sistema operativo que se puede conectar y administrar, sin embargo los contenedores son ligeros y están diseñados para crearse, escalarse horizontalmente y detenerse de forma dinámica. Aunque es posible crear e implementar máquinas virtuales a medida que aumenta la demanda de la aplicación, los contenedores están diseñados para permitirle responder a los cambios a petición. Con los contenedores, puede reiniciar rápidamente en caso de bloqueo o interrupción del hardware. Uno de los motores de contenedor más populares es Docker, que es compatible con Azure.

## Azure Container Instances
Azure Container Instances ofrece la forma más rápida y sencilla de ejecutar un contenedor en Azure, sin tener que administrar ninguna máquina virtual o adoptar ningún servicio adicional. Es una oferta de plataforma como servicio (PaaS) que permite cargar los contenedores, que se ejecutan automáticamente.

## Administrar contenedores
Los contenedores se administran a través de un orquestador de contenedores, que puede iniciar, detener y escalar horizontalmente las instancias de la aplicación, según sea necesario. Hay dos maneras de administrar los contenedores basados en Microsoft y Docker en Azure: Azure Container Instances y Azure Kubernetes Service (AKS).

## Azure Kubernetes Service
La tarea de automatizar y administrar una gran cantidad de contenedores (y de interactuar con ellos) se conoce como orquestación. Azure Kubernetes Service es un servicio completo de orquestación para contenedores con arquitecturas distribuidas y grandes volúmenes de contenedores.

## Decisión de cuándo usar Azure Functions

# Informatica sin servidor 

La informática sin servidor es la abstracción de los servidores, la infraestructura y los sistemas operativos. Con la informática sin servidor, Azure se encarga de administrar la infraestructura de servidor, así como de la asignación y desasignación de recursos según la demanda. La infraestructura no es responsabilidad del usuario. El escalado y el rendimiento se controlan automáticamente. Solo se le cobrarán los recursos exactos que use. Tampoco hay ninguna necesidad de reservar capacidad.
La informática sin servidor incluye la abstracción de servidores, un escalado controlado por eventos y la microfacturación:

- ***Abstracción de servidores:*** la informática sin servidor abstrae los servidores en los que se ejecuta. Nunca se reservan instancias de servidor de forma explícita. La plataforma las administra de forma automática. Cada ejecución de función puede ejecutarse en una instancia de proceso diferente. Este contexto de ejecución es transparente para el código. Con la arquitectura sin servidor, se implementa el código, el cual se ejecuta con alta disponibilidad.
- ***Escalado controlado por eventos:*** la informática sin servidor es una opción excelente para las cargas de trabajo que responden a eventos entrantes. Los eventos incluyen desencadenadores mediante lo siguiente:
  - Temporizadores, por ejemplo, si una función tiene que ejecutarse todos los días a las 10:00 UTC.
  - HTTP, por ejemplo, escenarios de API y webhook.
  - Colas, por ejemplo, con procesamiento de pedidos.
  - Y mucho más.
En lugar de escribir una aplicación completa, el desarrollador crea una función, la cual contiene código y metadatos sobre sus desencadenadores y enlaces. La plataforma programa automáticamente la función para que se ejecute y escala el número de instancias de proceso según la tasa de eventos de entrada. Los desencadenadores definen cómo se invoca una función. Los enlaces permiten conectarse de manera declarativa a servicios desde el código.
- Microfacturación: la informática tradicional factura para un bloque de tiempo, como el pago de una tarifa mensual o anual, para el hospedaje de sitios web. Este método de facturación es práctico, pero no siempre es rentable. Incluso si el sitio web de un cliente solo recibe una visita al día, este sigue pagando por tenerlo disponible durante todo el día. Con la informática sin servidor, solo se paga por el tiempo durante el que se ejecuta el código. Si no se produce ninguna ejecución de función activa, no se cobra al cliente. Por ejemplo, si el código se ejecuta una vez al día durante dos minutos, se le cobrará por una ejecución y por dos minutos de tiempo de proceso.

Azure tiene dos implementaciones de proceso sin servidor:

- ***Azure Functions:*** las funciones pueden ejecutar código en prácticamente cualquier lenguaje moderno.
- ***Azure Logic Apps:*** las aplicaciones lógicas están diseñadas en web y pueden ejecutar lógica desencadenada mediante servicios de Azure sin escribir código.
## Funciones
Functions es una opción ideal si le preocupa solo el código que ejecuta el servicio y no la infraestructura o la plataforma subyacente. Se usan normalmente cuando se debe realizar un trabajo en respuesta a un evento (a menudo a través de una solicitud REST), un temporizador o un mensaje de otro servicio de Azure, y cuando ese trabajo puede completarse rápidamente, en segundos o en menos tiempo.

## Azure Functions
El uso de Azure Functions es ideal si le preocupa solo el código que ejecuta el servicio, pero no la infraestructura o la plataforma subyacentes. Las funciones se usan normalmente cuando se debe realizar un trabajo en respuesta a un evento (a menudo a través de una solicitud REST), un temporizador o un mensaje de otro servicio de Azure, y cuando ese trabajo puede completarse rápidamente, en segundos o en menos tiempo.
Las funciones escalan automáticamente según la demanda, para que sean una opción sólida cuando la demanda es variable. Por ejemplo, podría recibir mensajes de una solución de IoT que se usa para supervisar una flota de vehículos de entrega. Probablemente llegarán más datos durante el horario comercial.

Mediante el uso de un enfoque basado en máquinas virtuales, incurrirá en costos incluso cuando la máquina virtual esté inactiva. Con Functions, Azure ejecuta el código cuando se desencadena y desasigna recursos automáticamente cuando la función finaliza. En este modelo, solo se le cobrará por el tiempo de CPU usado mientras se ejecuta la función.

Las funciones pueden ser sin estado o con estado. Cuando son sin estado (valor predeterminado), se comportan como si se reiniciaran cada vez que responden a un evento. Cuando son con estado (denominado Durable Functions), se pasa un contexto a través de la función para realizar el seguimiento antes de la actividad.

Las funciones son un componente clave de la informática sin servidor. También son una plataforma de proceso general para ejecutar cualquier tipo de código. Si cambian las necesidades de la aplicación del desarrollador, se puede implementar el proyecto en un entorno que no sea sin servidor. Esta flexibilidad permite administrar el escalado, ejecutar en redes virtuales e incluso aislar por completo las funciones.

## Azure Logic Apps
Las aplicaciones lógicas son similares a las funciones. Ambas permiten desencadenar lógica basada en un evento. Cuando las funciones ejecutan código, las aplicaciones lógicas ejecutan flujos de trabajo diseñados para automatizar escenarios empresariales y compilados a partir de bloques lógicos predefinidos.

Todos los flujos de trabajo de aplicación lógica de Azure comienza con un desencadenador, que se activa cuando se produce un evento específico o cuando hay nuevos datos disponibles que cumplen determinados criterios. Muchos desencadenadores incluyen funcionalidades de programación básicas que permiten a los desarrolladores especificar con qué frecuencia se ejecutarán sus cargas de trabajo. Cada vez que el desencadenador se activa, el motor de Logic Apps crea una instancia de aplicación lógica que ejecuta las acciones del flujo de trabajo. Estas acciones también pueden incluir conversiones de datos y controles de flujo, como instrucciones condicionales, instrucciones "switch", bucles y bifurcaciones.

Los flujos de trabajo de aplicaciones lógicas se crean mediante un diseñador visual en Azure Portal o en Visual Studio. Los flujos de trabajo se conservan como un archivo JSON con un esquema de flujo de trabajo conocido.

Azure proporciona más de 200 conectores y bloques de procesamiento diferentes para interactuar con servicios distintos. Estos recursos incluyen las aplicaciones empresariales más populares. También puede crear conectores personalizados y los pasos de flujo de trabajo si el servicio con el que necesita interactuar no está cubierto. Después, se usa el diseñador visual para vincular conectores y bloques. Los datos se pasan a través del flujo de trabajo para realizar el procesamiento personalizado, y todo ello a menudo sin escribir código.


## Azure Functions VS Azure Logic Apps
Functions y Logic Apps pueden crear orquestaciones complejas. Una orquestación es una colección de funciones o pasos que se ejecutan para realizar una tarea compleja.

- Con Functions, se escribe código para completar cada paso.
- Con Logic Apps, se usa una GUI para definir las acciones y cómo se relacionan entre sí.
Puede mezclar y combinar servicios cuando crea una orquestación, llamando a las funciones desde las aplicaciones lógicas y viceversa. Aquí se indican algunas diferencias comunes entre las dos.

![Funtions](https://user-images.githubusercontent.com/86896526/125179967-23757900-e1ba-11eb-936f-8ef0187ac0fa.JPG)


# ¿Qué es Azure Virtual Desktop?
Azure Virtual Desktop en Azure es un servicio de virtualización de escritorios y aplicaciones que se ejecuta en la nube. Permite que los usuarios usen una versión hospedada en la nube de Windows desde cualquier ubicación. Azure Virtual Desktop funciona en dispositivos como Windows, Mac, iOS, Android y Linux. Funciona con aplicaciones que se pueden usar para acceder a aplicaciones y escritorios remotos. También puede usar la mayoría de los exploradores modernos para acceder a experiencias hospedadas en Azure Virtual Desktop.

## Cacteristicas

## Administración simplificada
Azure Virtual Desktop es un servicio de Azure, por lo que resultará familiar para los administradores de Azure. Utilice Azure AD y RBAC para administrar el acceso a los recursos. Con Azure, también obtendrá herramientas para automatizar las implementaciones de máquinas virtuales, administrar las actualizaciones de máquinas virtuales y proporcionar recuperación ante desastres. Al igual que sucede con otros servicios de Azure, Azure Virtual Desktop usa Azure Monitor para la supervisión y las alertas. Esta estandarización permite a los administradores identificar incidencias con una única interfaz.

## Administración del rendimiento
Azure Virtual Desktop ofrece opciones para equilibrar la carga de los usuarios en los grupos de hosts de máquinas virtuales. Los grupos de hosts son colecciones de máquinas virtuales con la misma configuración asignada a varios usuarios. Para obtener el mejor rendimiento, puede configurar el equilibrio de carga para que se produzca cuando los usuarios inicien sesión (modo de amplitud). Con el modo de amplitud, los usuarios se asignan secuencialmente a través del grupo de hosts para la carga de trabajo. Para ahorrar costos, puede configurar las máquinas virtuales para el equilibrio de carga en modo de profundidad, donde los usuarios se asignan por completo en una máquina virtual antes de pasar a la siguiente. Azure Virtual Desktop proporciona herramientas para aprovisionar automáticamente máquinas virtuales adicionales cuando la demanda entrante supera un umbral especificado.

## Implementación de sesión múltiple de Windows 10
Azure Virtual Desktop permite usar la sesión múltiple de Windows 10 Enterprise, el único sistema operativo basado en cliente de Windows que permite varios usuarios simultáneos en una sola máquina virtual. Azure Virtual Desktop también proporciona una experiencia más coherente gracias a la compatibilidad más amplia con las aplicaciones en comparación con los sistemas operativos basados en Windows Server.

## Proporción de la mejor experiencia de usuario
Los usuarios tienen la libertad de conectarse a Azure Virtual Desktop con cualquier dispositivo a través de Internet. Emplean un cliente de Azure Virtual Desktop para conectarse a sus aplicaciones y escritorios de Windows publicados. Este cliente puede ser una aplicación nativa del dispositivo o el cliente web HTML5 de Azure Virtual Desktop.


### Aumento de la seguridad
Azure Virtual Desktop proporciona administración centralizada de la seguridad de los escritorios de los usuarios con Azure Active Directory (Azure AD). Puede habilitar la autenticación multifactor para proteger los inicios de sesión de los usuarios. También puede proteger el acceso a los datos mediante la asignación a los usuarios de controles de acceso basados en roles (RBAC) detallados.

Con Azure Virtual Desktop, los datos y las aplicaciones se separan del hardware local y se ejecutan en un servidor remoto. Se reduce el riesgo de dejar los datos confidenciales en un dispositivo personal.

Las sesiones de usuario están aisladas en entornos de una o varias sesiones.
