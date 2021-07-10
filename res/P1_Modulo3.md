# Parte 1 Modulo 3
## Suscripciones, los grupos de administración y los recursos de Azure
![cuentas](https://user-images.githubusercontent.com/86896526/125175470-0462f100-e192-11eb-9f55-a67a1533c229.png)
Una vez vista la jerarquía vertical de la organización, describamos cada uno de estos niveles empezando desde abajo:

- *Recursos:* elemento administrable que está disponible mediante Azure. Algunos ejemplos de recursos son las máquinas virtuales (VM), las cuentas de almacenamiento, las aplicaciones web, las bases de datos y las redes virtuales.
Los recursos son instancias de servicios que puede crear, como máquinas virtuales, almacenamiento o bases de datos SQL.
- *Grupos de recursos:* contenedor que incluye los recursos relacionados para una solución de Azure. El grupo de recursos incluye los recursos que se quieren administrar como grupo. Decida qué recursos pertenecen a un grupo de recursos según lo que más convenga a su organización.
Los recursos se combinan en grupos de recursos, que actúan como contenedor lógico en el que se implementan y administran recursos de Azure como aplicaciones web, bases de datos y cuentas de almacenamiento.
- *Suscripciones:* Una suscripción agrupa las cuentas de usuario y los recursos que han creado esas cuentas de usuario. Para cada suscripción, hay límites o cuotas en la cantidad de recursos que se pueden crear y usar. Las organizaciones pueden usar las suscripciones para administrar los costos y los recursos creados por los usuarios, equipos o proyectos.
- *Grupos de administración:* Estos grupos le ayudan a administrar el acceso, las directivas y el cumplimiento de varias suscripciones. Todas las suscripciones de un grupo de administración heredan automáticamente las condiciones que se aplican al grupo de administración.

## Zonas de  disponibilidad
Azure está formado por centros de datos ubicados en todo el mundo. Al usar un servicio o crear un recurso como una máquina virtual (VM) o una base de datos SQL, usa equipamiento físico en una o varias de estas ubicaciones. Estos centros de datos específicos no se exponen directamente a los usuarios, sino que Azure los organiza en regiones.
A fin de proteger la información en caso de error, deberá asegurarse de que los servicios y datos son redundantes. Si hospeda su infraestructura, configurar su propia redundancia requiere la creación de entornos de hardware duplicados. Azure puede ayudar a que la aplicación tenga alta disponibilidad a través de zonas de disponibilidad.
### ¿Qué es una zona de disponibilidad?
Las zonas de disponibilidad son centros de datos separados físicamente dentro de una región de Azure. Cada zona de disponibilidad consta de uno o varios centros de datos equipados con alimentación, refrigeración y redes independientes. Una zona de disponibilidad se configura para constituir un límite de aislamiento. Si una zona deja de funcionar, la otra continúa trabajando. Las zonas de disponibilidad están conectadas a través de redes de fibra óptica de alta velocidad privadas.

### Uso de las zonas de disponibilidad en sus aplicaciones
Si quiere usar zonas de disponibilidad para ejecutar aplicaciones críticas y conseguir una alta disponibilidad en la arquitectura de sus aplicaciones, coloque sus recursos de proceso, almacenamiento, red y datos dentro de una zona y replíquelos en otras. Tenga en cuenta que la duplicación de los servicios y la transferencia de datos entre zonas podrían suponer un costo.

Las zonas de disponibilidad son principalmente para las máquinas virtuales, los discos administrados, los equilibradores de carga y las bases de datos SQL. Los servicios de Azure que admiten zonas de disponibilidad se dividen en dos categorías:

- Servicios de zona: ancle el recurso a una zona específica (por ejemplo, máquinas virtuales, discos administrados, direcciones IP).
- Servicios de redundancia de zona: la plataforma se replica automáticamente entre zonas (por ejemplo, almacenamiento con redundancia de zona, SQL Database).


## Regiones de Azure
Una región es un área geográfica del planeta que contiene al menos un centro de datos, aunque podrían ser varios centros de datos cercanos y conectados mediante una red de baja latencia. Azure asigna y controla los recursos de forma inteligente dentro de cada región para garantizar que las cargas de trabajo están bien compensadas.
Algunos ejemplos de regiones son: Oeste de EE. UU., Centro de Canadá, Europa Occidental, Este de Australia y Japón Occidental. A continuación puede ver todas las regiones disponibles a fecha de junio de 2020.
![regiones](https://user-images.githubusercontent.com/86896526/125175528-72a7b380-e192-11eb-91a4-fd92caebc816.png)

 Las regiones globales proporcionan una mejor escalabilidad y redundancia, y conservan la residencia de datos para los servicios.
 
### Regiones de Azure especiales
Azure tiene regiones especializadas que se pueden usar al crear las aplicaciones, en lo referente al cumplimiento normativo o a aspectos legales. Algunos ejemplos incluyen:

- US DoD (centro), US Gov Virginia, US Gov Iowa y más: Estas regiones son instancias físicas y lógicas con aislamiento de red de Azure para asociados y agencias de la administración pública de EE. UU. Estos centros de datos están operados por personal estadounidense sometido a evaluación e incluyen certificaciones de cumplimiento adicionales.
- Este de China, Norte de China y más: Estas regiones están disponibles gracias a una asociación exclusiva entre Microsoft y 21Vianet, por la cual Microsoft no mantiene directamente los centros de datos.
Las regiones se utilizan para identificar la ubicación de los recursos, pero hay otros dos términos que también debe conocer: zonas geográficas y zonas de disponibilidad.

### Pares de regiones de Azure
Las zonas de disponibilidad se crean usando uno o varios centros de datos. Hay un mínimo de tres zonas en una sola región. Es posible que un desastre grande pueda provocar una interrupción tan grave como para afectar incluso a dos centros de datos. Por eso Azure también crea pares de regiones.
Puesto que las dos regiones están directamente conectadas y lo suficientemente lejos como para estar aisladas contra desastres regionales, puede usarlas para proporcionar redundancia de datos y servicios de confianza. Algunos servicios ofrecen un almacenamiento con redundancia geográfica automática utilizando los pares de regiones.

Ventajas adicionales de los pares de región:

- Si se produce una gran interrupción de Azure, se da prioridad a una región de cada par para asegurarse de que al menos una se restaure lo más rápido posible para las aplicaciones hospedadas en ese par de regiones.
- Las actualizaciones planeadas de Azure se implementan una a una en regiones emparejadas para minimizar el tiempo de inactividad y el riesgo de interrupción de la aplicación.
- Los datos siguen residiendo en la misma zona geográfica que su pareja (excepto Sur de Brasil) con fines de jurisdicción fiscal y de aplicación de la ley.
Tener un conjunto ampliamente distribuido de centros de datos permite a Azure proporcionar una alta garantía de disponibilidad.
![pares-de-region](https://user-images.githubusercontent.com/86896526/125175653-3032a680-e193-11eb-889b-262bda6d1009.png)


# Recursos 
 Un grupo de recursos es un contenedor lógico para recursos implementados en Azure. Estos recursos pueden ser cualquier cosa que cree en una suscripción de Azure como máquinas virtuales, instancias de Azure Application Gateway y de Azure Cosmos DB. Todos los recursos deben estar en un grupo de recursos, y un recurso solo puede ser miembro de un único grupo de recursos. Muchos recursos pueden moverse entre grupos de recursos con algunos servicios que tengan limitaciones o requisitos determinados para mover. Los grupos de recursos no se pueden anidar. Antes de poder aprovisionar un recurso, necesita un grupo de recursos en el que colocarlo.
 
 ## Agrupación lógica
Los grupos de recursos existen para ayudar a administrar y organizar los recursos de Azure. Al colocar recursos de uso, tipo o ubicación similar en un grupo de recursos, puede proporcionar orden y organización a los recursos que cree en Azure. La agrupación lógica es el aspecto que más le interesa, ya que, entre los recursos, el desorden es elevado.

### Ciclo de vida
Si elimina un grupo de recursos, también se eliminarán todos los recursos que contenga. La organización de los recursos por ciclo de vida puede ser útil en entornos que no sean de producción, en los que puede probar un experimento y después descartarlo. Los grupos de recursos facilitan la tarea de quitar un conjunto de recursos a la vez.

### Autorización
Los grupos de recursos también son un ámbito para aplicar permisos de control de acceso basado en roles (RBAC). Al aplicar permisos RBAC a un grupo de recursos, puede facilitar la administración y limitar el acceso para permitir solo lo que sea necesario.

## Azure Resource Manager
Azure Resource Manager es el servicio de implementación y administración para Azure. Proporciona una capa de administración que le permite crear, actualizar y eliminar recursos de la cuenta de Azure. Puede usar características de administración como el control de acceso, los bloqueos y las etiquetas para proteger y organizar los recursos después de la implementación.

Cuando un usuario envía una solicitud de cualquiera de las herramientas, las API o los SDK de Azure, Resource Manager recibe la solicitud. Autentica y autoriza la solicitud. Resource Manager envía la solicitud al servicio de Azure, que lleva a cabo la acción solicitada. Dado que todas las solicitudes se controlan mediante la misma API, verá resultados y funcionalidades coherentes en todas las distintas herramientas.

### Ventajas de usar Administrador de recursos
Con Resource Manager puede:

- Administrar la infraestructura mediante plantillas declarativas en lugar de scripts. Una plantilla de Resource Manager es un archivo JSON que define lo que quiere implementar en Azure.
- Implementar, administrar y supervisar todos los recursos de la solución en grupo, en lugar de controlarlos individualmente.
- Vuelva a implementar la solución a lo largo del ciclo de vida de desarrollo y tenga la seguridad de que los recursos se implementan en un estado coherente.
- Definir las dependencias entre recursos de modo que se implementen en el orden correcto.
- Aplique control de acceso a todos los servicios, puesto que RBAC se integra de forma nativa en la plataforma de administración.
- Aplicar etiquetas a los recursos para organizar de manera lógica todos los recursos de la suscripción.
- Comprenda la facturación de la organización viendo los costos de un grupo de recursos que comparten la misma etiqueta.

# Subscripcones y Grupos de administración
## Subscripción Azure
El uso de Azure requiere una suscripción de Azure. Una suscripción le proporciona acceso autenticado y autorizado a los servicios y productos de Azure. Además, también le permite aprovisionar los recursos. Una suscripción de Azure es una unidad lógica de servicios de Azure que está vinculada a una cuenta de Azure, que es una identidad en Azure Active Directory (Azure AD) o en un directorio en el que confía Azure AD.
![subcripcion](https://user-images.githubusercontent.com/86896526/125175806-3412f880-e194-11eb-8946-9b67a6bbb15f.png)

Una cuenta puede tener una suscripción o varias suscripciones que con distintos modelos de facturación y a las que se aplican diferentes directivas de administración de acceso. Puede usar las suscripciones de Azure para definir límites en torno a los productos, servicios y recursos de Azure. Hay dos tipos de límites de suscripción que puede utilizar:

- Límite de facturación: Este tipo de suscripción determina cómo se factura una cuenta de Azure por el uso de Azure. Puede crear varias suscripciones para diferentes tipos de requisitos de facturación. Azure genera facturas e informes de facturación independientes para cada suscripción, de modo que pueda organizar y administrar los costos.
- Límite de control de acceso: Azure aplica las directivas de administración de acceso en el nivel de suscripción, por lo que puede crear suscripciones independientes para reflejar distintas estructuras organizativas. Por ejemplo, dentro de una empresa hay diferentes departamentos a los que se pueden aplicar directivas de suscripción de Azure distintas. Este modelo de facturación le permite administrar y controlar el acceso a los recursos que los usuarios aprovisionan con suscripciones específicas.

## Creación de una suscripción de Azure adicional
Es posible que quiera crear suscripciones adicionales para fines de administración de facturación o de recursos. Por ejemplo, puede optar por crear suscripciones adicionales para separar lo siguiente:

- Entornos: cuando administra sus recursos, puede optar por crear suscripciones con el fin de configurar entornos independientes para el desarrollo y las pruebas, para seguridad o para aislar los datos por motivos de cumplimiento. Este diseño es especialmente útil porque el control de acceso a los recursos se produce en el nivel de suscripción.
- Estructuras organizativas: puede crear suscripciones para reflejar las distintas estructuras organizativas. Por ejemplo, podría limitar un equipo a recursos de bajo costo, al tiempo que permite que el departamento de TI tenga un alcance completo. Este diseño permite administrar y controlar el acceso a los recursos que los usuarios aprovisionan en cada suscripción.
- Facturación: es posible que también quiera crear suscripciones adicionales para fines de facturación. Dado que los costos se agregan primero en el nivel de suscripción, es posible que quiera crear suscripciones para administrar y realizar un seguimiento de los costos en función de sus necesidades. Por ejemplo, puede que quiera crear una suscripción para las cargas de trabajo de producción, y otra suscripción para las cargas de trabajo de desarrollo y pruebas.
Es posible que también necesite suscripciones adicionales debido a lo siguiente:

Límites de suscripción: las suscripciones se enlazan a algunas limitaciones de hardware. Por ejemplo, el número máximo de circuitos de Azure ExpressRoute por cada suscripción es de 10. Esos límites se deben tener en consideración al crear suscripciones en la cuenta. Si en escenarios concretos hay que superar esos límites, es posible que se necesiten suscripciones adicionales

## Grupos de administración de Azure
Si la organización tiene muchas suscripciones, es posible que necesite una forma de administrar con eficacia el acceso, las directivas y el cumplimiento para esas suscripciones. Los grupos de administración de Azure ofrecen un nivel de ámbito que está por encima de las suscripciones. Las suscripciones se organizan en contenedores llamados grupos de administración y las condiciones de gobernanza se aplican a los grupos de administración. Todas las suscripciones dentro de un grupo de administración heredan automáticamente las condiciones que se aplican al grupo de administración. Los grupos de administración proporcionan capacidad de administración de nivel empresarial a gran escala con independencia del tipo de suscripciones que tenga. Todas las suscripciones de un único grupo de administración deben confiar en el mismo inquilino de Azure AD.

## Jerarquía de los grupos de administración y las suscripciones
Puede compilar una estructura flexible de grupos de administración y suscripciones para organizar los recursos en una jerarquía para una administración unificada de las directivas y el acceso. El diagrama siguiente muestra un ejemplo de creación de una jerarquía para la gobernanza mediante grupos de administración.
![gestion-grupos-subcripciones](https://user-images.githubusercontent.com/86896526/125175859-adaae680-e194-11eb-8aea-88bfe231a01a.png)
Puede crear una jerarquía que aplique una directiva. Por ejemplo, puede limitar las ubicaciones de las máquinas virtuales a la región oeste de EE. UU. en un grupo denominado Producción. Esta directiva se heredará en todas suscripciones de Contrato Enterprise que sean descendientes de ese grupo de administración y se aplicará a todas las máquinas virtuales de esas suscripciones. El propietario de los recursos o las suscripciones no puede modificar esta directiva de seguridad, lo que permite una gobernanza mejorada.

## Hechos importantes acerca de los grupos de administración
* Se admiten 10 000 grupos de administración en un único directorio.
* Un árbol de grupo de administración puede admitir hasta seis niveles de profundidad. Este límite no incluye el nivel raíz ni el nivel de suscripción.
* Cada grupo de administración y suscripción solo puede admitir un elemento primario.
* Cada grupo de administración puede tener muchos elementos secundarios.
* Todas las suscripciones y grupos de administración están dentro de una única jerarquía en cada directorio.


# Dentro del portal de AZURE
## ¿Qué es App Service?
App Service es un servicio basado en HTTP que permite crear y hospedar muchos tipos de soluciones basadas en la Web sin necesidad de administrar la infraestructura. Por ejemplo, puede hospedar aplicaciones web, back-ends móviles y API de RESTful en varios lenguajes de programación admitidos. Las aplicaciones desarrolladas en .NET, .NET Core, Java, Ruby, Node.js, PHP o Python se pueden ejecutar y escalar con facilidad en entornos basados tanto en Windows como en Linux.

## ¿Qué es Azure Marketplace?
Azure Marketplace es una tienda en línea que hospeda aplicaciones certificadas y optimizadas para ejecutarse en Azure. Existen muchos tipos de aplicaciones disponibles, que van desde la inteligencia artificial y Machine Learning a las aplicaciones web. Como veremos en un par de minutos, las implementaciones desde la tienda se realizan mediante Azure Portal, con una interfaz de usuario de tipo asistente. Esta interfaz de usuario permite evaluar fácilmente diferentes soluciones.

## Creación de recursos en Azure
Lo primero que se suele hacer es crear un grupo de recursos que contendrá todo lo que necesitamos crear. El grupo de recursos nos permite administrar todos los servicios, discos, interfaces de red y demás elementos que pueden conformar la solución como una unidad. Podemos usar Azure Portal para crear y administrar los grupos de recursos de la solución, pero tenga en cuenta que también puede administrar recursos a través de una línea de comandos con la CLI de Azure. La CLI de Azure es una opción útil si hay que automatizar el proceso en el futuro.

En el entorno de espacio aislado gratuito de Azure, usará el grupo de recursos creado previamente, [nombre del grupo de recursos del espacio aislado], por lo que no tendrá que realizar este paso.
