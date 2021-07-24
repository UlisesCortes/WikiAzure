# Parte 6 Modulo 19
La calculadora de TCO le ayuda a calcular los costos que se ahorra al hacer funcionar la solución en Azure con el tiempo, en lugar de hacerlo en el centro de datos local.

El término costo total de propiedad se usa normalmente en finanzas. Puede ser difícil ver todos los costos ocultos relacionados con el funcionamiento de una capacidad tecnológica en el entorno local. Las licencias de software y el hardware son costos adicionales.

El trabajo con la calculadora de TCO involucra tres pasos:

Definir las cargas de trabajo
Ajustar los supuestos
Consulte el informe.

## Paso 1: Definir las cargas de trabajo
En primer lugar, escriba las especificaciones de la infraestructura local en la calculadora de TCO, en función de estas cuatro categorías:

- Servidores
Esta categoría incluye los sistemas operativos, los métodos de virtualización, los núcleos de CPU y la memoria (RAM).

- Bases de datos
Esta categoría incluye los tipos de base de datos, el hardware de servidores y el servicio de Azure que quiere usar, incluidos los inicios de sesión de usuario simultáneos máximos esperados.

- Storage
Esta categoría incluye el tipo y la capacidad de almacenamiento, incluida toda copia de seguridad o almacenamiento de archivo.

- Redes
Esta categoría incluye la cantidad de ancho de banda de red que se usa actualmente en el entorno local.

## Paso 2: Ajustar supuestos
A continuación, especifique si las licencias locales actuales están inscritas para Software Assurance, lo cual puede ayudarle a ahorrar dinero al reutilizar esas licencias en Azure. También se especifica si es necesario replicar el almacenamiento en otra región de Azure para obtener una mayor redundancia.

* Precio de electricidad por kilovatios/hora (KWh).
* Tarifa por hora para la administración de TI.
* Costo de mantenimiento de la red como un porcentaje de los costos de software y hardware de red.
Para mejorar la precisión de los resultados de la calculadora de TCO, debe ajustar los valores para que coincidan con los costos de la infraestructura local actual.


## Paso 3: Ver el informe
Elija un período de tiempo entre uno y cinco años. La calculadora de TCO genera un informe que se basa en la información especificada.

Para cada categoría (proceso, centro de datos, redes, almacenamiento y personal de TI), también puede ver una comparación en paralelo del desglose de costos de funcionamiento de esas cargas de trabajo locales frente a su funcionamiento en Azure.


# Aspectos a tomar en cuenta en la estimaión de costos
## ¿Qué tipos de suscripciones de Azure puedo usar?
Probablemente sepa que una suscripción de Azure le proporciona acceso a los recursos de Azure, como máquinas virtuales (VM), almacenamiento y bases de datos. Los tipos de recursos que use afectan a su factura mensual.

* Evaluación gratuita
Una suscripción de evaluación gratuita proporciona 12 meses de servicios gratuitos populares, un crédito para explorar cualquier servicio de Azure durante 30 días y más de 25 servicios que siempre son gratis.

* Pago por uso
Una suscripción de pago por uso le permite pagar por lo que usa al conectar una tarjeta de crédito o débito a su cuenta. Las organizaciones pueden solicitar descuentos por volumen y facturación de pago por adelantado.

* Ofertas para miembros
La pertenencia existente a determinados productos y servicios de Microsoft puede proporcionarle créditos para su cuenta de Azure y tarifas reducidas en los servicios de Azure.

## ¿Cómo compro servicios de Azure?
* A través de un Contrato Enterprise
Los clientes más grandes, conocidos como clientes empresariales, pueden firmar una Contrato Enterprise con Microsoft. Este contrato los compromete a gastar una cantidad predeterminada en los servicios de Azure durante un período de tres años. Normalmente, el precio de los servicios se paga anualmente. 

* Directamente desde la web
Aquí se compran los servicios de Azure directamente desde el sitio web de Azure Portal y se pagan precios estándar. Se factura mensualmente, como un pago de tarjeta de crédito o a través de una factura. Este método de compra se conoce como Web Direct.

*A través de un Proveedor de soluciones en la nube
Un Proveedor de soluciones en la nube (CSP) es un partner de Microsoft que le ayuda a crear soluciones a partir de Azure. El CSP le factura por el uso de Azure a un precio determinado. También responde a las preguntas de soporte técnico y las remite a Microsoft según sea necesario.


## ¿Qué factores afectan al costo?
La forma en que usa sus recursos, el tipo de suscripción y los precios de los proveedores de terceros son factores comunes. Examinemos rápidamente cada uno.

* Tipo de recurso
Varios factores influyen en el costo de los recursos de Azure. Dependen del tipo de recurso o de cómo se personalice.

* Medidores de uso
Al aprovisionar un recurso, Azure crea medidores para realizar el seguimiento del uso de dicho recurso. Azure usa estos medidores para generar un registro de uso que posteriormente se usa para ayudar a calcular la factura.
El uso del que un medidor realiza el seguimiento se correlaciona con una cantidad de unidades facturables. Estas unidades se cobran en su cuenta por cada período de facturación. La tarifa por cada unidad facturable depende del tipo de recurso que use.

Piense en los medidores de uso de forma similar a la forma en que usa electricidad o agua en su hogar. Puede que pague un precio base cada mes por el servicio de electricidad o de agua, pero su factura final se basa en la cantidad total que consuma.
Los siguientes tipos de medidores son pertinentes para el seguimiento de su uso:

- Tiempo total de CPU.
- Tiempo empleado en una dirección IP pública.
- Tráfico de red entrante (entrada) y saliente (salida) de la máquina virtual.
- Tamaño del disco y cantidad de operaciones de lectura y escritura del disco.

* Uso de recursos
En Azure, siempre se le cobrará en función de lo que use. Por ejemplo, echemos un vistazo a la forma en que esta facturación se aplica para desasignar una VM.

* Tipos de suscripción de Azure
Algunos tipos de suscripciones de Azure también incluyen provisiones de uso que afectan a los costos.

* Azure Marketplace
También puede comprar a otros proveedores soluciones y servicios basados en Azure a través de Azure Marketplace. Entre los ejemplos se incluyen conectores o dispositivos de firewall de red administrada para servicios de copia de seguridad de terceros. El proveedor establece las estructuras de facturación.

## ¿Afecta el tráfico de red o la ubicación al costo?
* Location
La infraestructura de Azure se distribuye globalmente, lo cual permite implementar los servicios de forma centralizada o aprovisionar los servicios más cercanos al lugar donde los clientes los usan.

* Zonas para la facturación del tráfico de red
Las zonas de facturación son un factor a la hora de determinar el costo de algunos servicios de Azure.

El ancho de banda hace referencia a los datos que entran y salen de los centros de datos de Azure. Algunas transferencias de datos entrantes (datos que se dirigen a los centros de datos de Azure) son gratis. En cuanto a las transferencias de datos salientes (datos que salen de los centros de datos de Azure), el precio de la transferencia de datos se basa en las zonas.

Una zona es una agrupación geográfica de regiones de Azure para fines de facturación. Las siguientes zonas incluyen algunas de las regiones que se muestran aquí:

- * Zona 1: Centro de Australia, Oeste de EE. UU., Este de EE. UU., Oeste de Canadá, Oeste de Europa, Centro de Francia y otras
- * Zona 2: Este de Australia, Japón Occidental, Centro de la India, Sur de Corea del Sur y otras
- * Zona 3: Sur de Brasil, Norte de Sudáfrica, Oeste de Sudáfrica, Centro de Emiratos Árabes Unidos, Norte de Emiratos Árabes Unidos
- * Zona 1 de Alemania: Centro de Alemania y Nordeste de Alemania

## ¿Cómo puedo calcular el costo total?
La Calculadora de precios muestra los productos de Azure por categorías. Agregue estas categorías a su estimación y configúrelas según sus requisitos específicos. Luego recibirá un precio estimado consolidado, con un desglose detallado de los costos asociados a cada recurso que ha agregado a la solución. Puede exportar o compartir esa estimación o guardarla para más adelante. Puede cargar una estimación guardada y modificarla para que coincida con los requisitos actualizados.

Las opciones que se pueden configurar en la Calculadora de precios varían entre productos, pero pueden incluir:

* Región
* Nivel
* Opciones de facturación
* Opciones de soporte técnico
* Programas y ofertas
* Precios de Desarrollo/pruebas de Azure

# Administrar y minimizar el costo total en Azure
* Comprender los costos estimados antes de implementar
Calcule los costos previstos mediante la Calculadora de precios y la calculadora de costo total de propiedad (TCO). Agregue solo los productos, servicios y recursos que necesita para la solución.

* Usar Azure Advisor para supervisar la utilización
Azure Advisor identifica los recursos no utilizados o infrautilizados, y recomienda recursos no utilizados que se pueden quitar. Esta información le ayudará a configurar los recursos para que coincidan con la carga de trabajo real.

* Usar límites de gasto para restringir los gastos
Si tiene una evaluación gratuita o una suscripción de Azure basada en crédito, puede usar los límites de gasto para evitar la saturación accidental.
Si tiene una suscripción basada en crédito y alcanza el límite de gasto configurado, Azure suspende su suscripción hasta que comience un nuevo período de facturación.

* Usar Reservas de Azure para pagar por adelantado
Reservas de Azure ofrecen precios con descuento en determinados servicios de Azure. Reservas de Azure puede ahorrar hasta un 72 % en comparación con los precios de pago por uso. Para recibir un descuento, reserve los servicios y recursos abonándolos por adelantado.

* Elegir regiones y ubicaciones de bajo costo
El costo de los productos, servicios y recursos de Azure puede variar entre ubicaciones y regiones. Si es posible, debe usarlos en aquellas ubicaciones y regiones donde el costo es menor.

### * Usar Azure Cost Management + Billing para controlar gastos
Azure Cost Management + Billing es un servicio gratuito que le ayuda a comprender su factura de Azure, administrar su cuenta y sus suscripciones, supervisar y controlar los gastos de Azure, y optimizar el uso de recursos.
Las características de Azure Cost Management + Billing incluyen:

- Reporting
Use datos históricos para generar informes y predecir el uso y los gastos futuros.

- Enriquecimiento de datos
Mejore la responsabilidad mediante la categorización de los recursos con etiquetas que se correspondan con las unidades organizativas y empresariales del mundo real.

- Presupuestos
Cree y administre presupuestos de costos y uso mediante la supervisión de tendencias de demanda de recursos, tasas de consumo y patrones de costos.

- Alertas
Obtenga alertas basadas en los presupuestos de costos y uso.

- Recomendaciones
Reciba recomendaciones para eliminar recursos inactivos y para optimizar los recursos de Azure que aprovisiona.

### Aplicar etiquetas para identificar a los propietarios de costos
Las etiquetas ayudan a administrar los costos asociados a los distintos grupos de productos y recursos de Azure. Puede aplicar etiquetas a grupos de recursos de Azure para organizar los datos de facturación.

### Cambiar el tamaño de las máquinas virtuales infrautilizadas
Una recomendación común que encontrará de Azure Cost Management + Billing y Azure Advisor es cambiar el tamaño o apagar las VM que están infrautilizadas o inactivas.

### Desasignar máquinas virtuales durante las horas de inactividad
Recuerde que desasignar una máquina virtual significa que ya no se ejecuta la máquina virtual, sino que se conservan los discos duros y los datos asociados en Azure.

### Eliminar recursos no utilizados
Es posible que esta recomendación parezca obvia, pero, si no usa un recurso, debería apagarlo. No es poco frecuente encontrar sistemas de prueba de concepto, o que no son de producción, que después de completar un proyecto ya no son necesarios.

# Extra RESUMEN
La lista incluye lo siguiente:

Realizar un análisis de costos antes de la implementación.
Usar Azure Advisor para supervisar la utilización.
Usar los límites de gasto para evitar gastos accidentales.
Usar Reservas de Azure para pagar por adelantado.
Elegir regiones y ubicaciones de bajo costo.
Investigar las ofertas de ahorro de costos disponibles.
Aplicar etiquetas para identificar a los propietarios de costos.

### Comprar servicios de Azure
- Si acaba de empezar a usar Azure, revise las preguntas más frecuentes sobre la cuenta gratuita de Azure para ver si una cuenta de evaluación gratuita es la adecuada para usted.
- Para obtener más información sobre cómo comprar productos y servicios de Azure, vea Exploración de opciones de compra flexibles para Azure.

## Descripción de la factura
Para obtener más información sobre los cargos de uso de Azure, vea Descripción de los términos en su factura de Microsoft Azure.
Para obtener más información sobre cómo afecta el ancho de banda a los precios, consulte Detalles de precios de ancho de banda.

## Administrar y minimizar los costos
Vea Azure Cost Management + Billing para obtener más información sobre el análisis de costos, la creación y administración de presupuestos, la exportación de datos y la revisión y actuación según recomendaciones.
Aproveche los importantes descuentos en las cargas de trabajo de desarrollo y pruebas. Para obtener más información, consulte Precios de Desarrollo/pruebas de Azure.
Obtenga más información sobre cómo Reservas de Azure puede ayudarle a ahorrar dinero cuando se compromete a planes de tarifa de uno o tres años.
Obtenga información sobre cómo evitar cargos inesperados con la administración de costos y facturación de Azure.
Vea Límite de gasto de Azure para saber lo que sucede cuando se alcanza el límite de gasto y cómo quitarlo.
Obtenga información sobre cómo iniciar y detener máquinas virtuales fuera de las horas de trabajo.
Vea cómo la Ventaja híbrida de Azure puede ayudar a ahorrar costos incorporando a Azure las licencias de Windows Server y SQL Server locales con Software Assurance.




