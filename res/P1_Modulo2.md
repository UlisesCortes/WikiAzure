# Parte 1 Modulo 2
## ¿Qué son las nubes pública, privada e híbrida?
Hay tres modelos de implementación para la informática en la nube: nube pública, nube privada y nube híbrida. Cada modelo de implementación tiene distintos aspectos que debe tener en cuenta a la hora de migrar a la nube.


Nombre de Implementación | Función del servicio
--------- | -----------
[Nube pública](#nube-publica) | Los servicios se ofrecen a través de la red Internet pública y están disponibles para cualquiera que quiera comprarlos. Los recursos de nube, como los servidores y el almacenamiento, son propiedad de un proveedor de servicios en la nube de terceros, que los explota y los distribuye a través de Internet.
[Nube privada](#nube-privada) | Una nube privada consta de recursos informáticos que determinados usuarios de una empresa u organización usan en exclusiva. Una nube privada puede estar ubicada físicamente en el centro de datos local (entorno local) de la organización o estar hospedada por un proveedor de servicios de terceros.
[Nube híbrida](#nube-hibrida) | Una nube híbrida es un entorno informático que combina una nube pública y una nube privada, lo que permite compartir datos y aplicaciones entre ellas.

Comparación de modelos de nube

Nube pública
* No hay gastos de capital para escalar verticalmente.
* Las aplicaciones pueden aprovisionarse y desaprovisionarse rápidamente.
* Las organizaciones solo pagan por lo que usan.

Nube privada

* Debe adquirirse hardware para el inicio y el mantenimiento.
* Las organizaciones tienen un control total de los recursos y la seguridad.
* Las organizaciones son responsables del mantenimiento y las actualizaciones del hardware.

Nube híbrida
* Proporciona la máxima flexibilidad.
* Las organizaciones determinan dónde se van a ejecutar sus aplicaciones.
*Las organizaciones controlan la seguridad, el cumplimiento o los requisitos legales.


## ¿Cuáles son algunas de las ventajas de la informática en la nube?
Los entornos en la nube ofrecen varias ventajas en comparación con los entornos físicos. Tailwind Traders puede aprovecharlas después de su migración a Azure.

- Alta disponibilidad: en función del contrato de nivel de servicio (SLA) que elija, las aplicaciones basadas en la nube pueden proporcionar una experiencia de usuario continua sin tiempo de inactividad perceptible, aunque se produzcan errores.

- Escalabilidad: las aplicaciones en la nube se pueden escalar verticalmente y horizontalmente:

- *Escale verticalmente para aumentar la capacidad de proceso mediante la incorporación de RAM o CPU adicionales a una máquina virtual.
- * El escalado horizontal aumenta la capacidad de proceso mediante la adición de instancias de recursos, como la incorporación de máquinas virtuales a la configuración.

- Elasticidad: puede configurar aplicaciones basadas en la nube para aprovechar el escalado automático, de forma que las aplicaciones siempre dispondrán de los recursos que necesitan.

- Agilidad: implemente y configure rápidamente los recursos basados en la nube a medida que cambian los requisitos de la aplicación.

- Distribución geográfica: puede implementar aplicaciones y datos en centros de datos regionales de todo el mundo, lo que garantiza que sus clientes siempre tendrán el mejor rendimiento de su región.

- Recuperación ante desastres: al usar los servicios de copia de seguridad basados en la nube, la replicación de datos y la distribución geográfica, podrá implementar las aplicaciones con la seguridad de saber que los datos están protegidos en caso de que se produzca un desastre.

## Gastos de capital en comparación con los gastos operativos
Hay dos tipos diferentes de gastos que se deben tener en cuenta:

- Los gastos de capital (CapEx) hacen referencia a la inversión previa de dinero en infraestructura física, que se podrá deducir a lo largo del tiempo. El costo previo de CapEx tiene un valor que disminuye con el tiempo.

- Los gastos operativos (OpEx) son dinero que se invierte en servicios o productos y se factura al instante. Este gasto se puede deducir el mismo año que se produce. No hay ningún costo previo, ya que se paga por un servicio o producto a medida que se usa.

Dicho de otra forma, si Tailwind Traders es dueño de su infraestructura, comprará equipos que se incluirán como recursos en su balance de cuentas. Dado que se ha realizado una inversión de capital, los contables clasifican esta transacción como CapEx. Con el tiempo, a fin de contabilizar la duración útil limitada de los activos, estos se deprecian o se amortizan.

Los servicios en la nube, por otro lado, se clasifican como OpEx debido a su modelo de consumo. No hay ningún recurso que Tailwind Traders pueda amortizar, y su proveedor de servicios en la nube (Azure) administra los costos asociados con la compra y la vida útil del equipo físico. En consecuencia, los gastos de explotación tienen un impacto directo en el beneficio neto, la base imponible y los gastos asociados en el balance contable.

En resumen, CapEx requiere unos costos financieros previos considerables, así como unos gastos continuos de mantenimiento y soporte técnico. En cambio, OpEx es un modelo basado en el consumo, así que Tailwind Traders solo es responsable del costo de los recursos informáticos que utiliza.

## La informática en la nube es un modelo basado en el consumo
Los proveedores de servicios en la nube operan en un modelo basado en el consumo, lo que significa que los usuarios finales solo pagan por los recursos que usan. Lo que usan es lo que pagan.

Los modelos basados en el consumo aportan muchas ventajas, por ejemplo:

- Sin costes por adelantado.
- No es necesario comprar ni administrar infraestructuras costosas que es posible que los usuarios no aprovechen del todo.
- Se puede pagar para obtener recursos adicionales cuando se necesiten.
- Se puede dejar de pagar por los recursos que ya no se necesiten.


## ¿Qué son los modelos de servicio en la nube?

Si hace tiempo que tiene conocimientos sobre la informática en la nube, es probable que haya visto los acrónimos PaaS, IaaS y SaaS de los diferentes modelos de servicio en la nube. Estos modelos definen los diferentes niveles de responsabilidad compartida de un proveedor de nube y un inquilino de nube.

Modelo | Descripción
--------- | -----------
IaaS - Infraestructura como servicio | Este modelo de servicio en la nube es el más similar a la administración de servidores físicos; un proveedor de servicios en la nube mantendrá actualizado el hardware, pero el mantenimiento del sistema operativo y la configuración de red serán su responsabilidad como inquilino de nube. Por ejemplo, las máquinas virtuales de Azure son dispositivos de proceso virtuales totalmente operativos que se ejecutan en centros de datos de Microsoft. Una ventaja de este modelo de servicio en la nube es la rápida implementación de nuevos dispositivos de proceso. Configurar una máquina virtual nueva es considerablemente más rápido que obtener, instalar y configurar un servidor físico.
PaaS - Plataforma como servicio | Este modelo de servicio en la nube es un entorno de hospedaje administrado. El proveedor de servicios en la nube administra las máquinas virtuales y los recursos de red, y el inquilino de nube implementa sus aplicaciones en el entorno de hospedaje administrado. Por ejemplo, Azure App Services proporciona un entorno de hospedaje administrado en el que los desarrolladores pueden cargar sus aplicaciones web sin tener que preocuparse por los requisitos de hardware y software físicos.
SaaS - Software como servicio | En este modelo de servicio en la nube, el proveedor de servicios en la nube administra todos los aspectos del entorno de la aplicación, como las máquinas virtuales, los recursos de red, el almacenamiento de datos y las aplicaciones. El inquilino de nube solo necesita proporcionar sus datos a la aplicación administrada por el proveedor de servicios en la nube. Por ejemplo, Microsoft Office 365 proporciona una versión de Microsoft Office totalmente operativa que se ejecuta en la nube. Lo único que debe hacer es crear el contenido, y Office 365 se encargará de todo lo demás.

## COMPARACIÓN
### IaaS
IaaS es la categoría más flexible de servicios en la nube. Su objetivo es ofrecer un control completo sobre el hardware que ejecuta la aplicación. En vez de comprar hardware, con IaaS, se alquila.

Ventajas
- Sin gastos de capital (CapEx). Los usuarios no tienen costos iniciales.

- Agilidad. Se pueden configurar las aplicaciones con rapidez para que sean accesibles y desaprovisionarlas cuando sea necesario.

- Administración. Se aplica el modelo de responsabilidad compartida; el usuario administra y mantiene los servicios que ha aprovisionado, y el proveedor de nube administra y mantiene la infraestructura en la nube.

- Modelo basado en el consumo. Las organizaciones solo pagan por lo que usan y operan en un modelo de gastos operativos (OpEx).

- Aptitudes. No se requieren conocimientos técnicos avanzados para implementar y usar una nube pública u obtener las ventajas que esta ofrece. Las organizaciones pueden utilizar las aptitudes y la experiencia del proveedor de nube para asegurarse de que las cargas de trabajo sean seguras, estén protegidas y tengan alta disponibilidad.

- Ventajas que ofrece la nube. Las organizaciones pueden utilizar las aptitudes y la experiencia del proveedor de nube para asegurarse de que las cargas de trabajo se configuren de forma que sean seguras y tengan alta disponibilidad.

- Flexibilidad. IaaS es el servicio en la nube más flexible, ya que se dispone de control para configurar y administrar el hardware que ejecuta una aplicación.

### PaaS
PaaS proporciona las mismas ventajas y consideraciones que IaaS, pero ofrece algunas ventajas adicionales que es importante conocer.

- *Ventajas
Sin gastos de capital (CapEx). Los usuarios no tienen costos iniciales.

- Agilidad. PaaS es más ágil que IaaS, y no es necesario que los usuarios configuren servidores para ejecutar aplicaciones.

- Modelo basado en el consumo. Los usuarios solo pagan por lo que usan y operan bajo un modelo OpEx.

- Aptitudes. No se requieren conocimientos técnicos avanzados para implementar y usar una plataforma PaaS u obtener las ventajas que esta ofrece.

- Ventajas que ofrece la nube. Los usuarios pueden aprovechar las aptitudes y la experiencia del proveedor de nube para asegurarse de que sus cargas de trabajo sean seguras y tengan alta disponibilidad. Además, los usuarios pueden obtener acceso a más herramientas de desarrollo punteras. Entonces, las podrán aplicar al ciclo de vida de una aplicación.

- Productividad. Los usuarios se pueden centrar únicamente en el desarrollo de aplicaciones, ya que el proveedor de nube lleva a cabo toda la administración de plataformas. Trabajar con equipos distribuidos como servicios es más fácil, ya que se accede a la plataforma a través de Internet. Puede hacer que la plataforma esté disponible globalmente de forma más sencilla.

- *Desventaja
Limitaciones de la plataforma. Es posible que en las plataformas en la nube haya una serie de limitaciones que pueden afectar al modo en el que una aplicación se ejecuta. Al evaluar qué plataforma PaaS es más adecuada para una carga de trabajo, debe tener en cuenta las limitaciones de esta área.

### SaaS
SaaS es software que se hospeda y administra de forma centralizada para usted y sus usuarios o clientes. Normalmente se usa una versión de la aplicación para todos los clientes y la licencia se obtiene mediante una suscripción mensual o anual.

- SaaS proporciona las mismas ventajas que IaaS, pero también ofrece algunas ventajas adicionales que es importante conocer.

- *Ventajas
Sin gastos de capital (CapEx). Los usuarios no tienen costos iniciales.

- Agilidad. Los usuarios pueden proporcionar al personal acceso al software más reciente de forma fácil y rápida.

- Modelo de precio de pago por uso. Los usuarios pagan por el software que usan mediante un modelo de suscripción, que habitualmente es mensual o anual, independientemente de cuánto usen el software.

- Aptitudes. No se requieren conocimientos técnicos avanzados para implementar y usar software SaaS u obtener las ventajas que este ofrece.

- Flexibilidad. Los usuarios pueden acceder a los mismos datos de la aplicación desde cualquier lugar.

- *Desventaja
- Limitaciones de software. Es posible que en las aplicaciones de software haya una serie de limitaciones que pueden afectar al modo en el que los usuarios trabajan. Como está usando el software tal cual, no tiene un control directo de las características. Al evaluar qué plataforma SaaS es más adecuada para una carga de trabajo, debe tener en cuenta cualquier necesidad empresarial y las limitaciones de software.

Comparación de modelos de servicio en la nube

IaaS 
El servicio en la nube más flexible. 
Configure y administre el hardware de la aplicación.

PaaS
Céntrese en el desarrollo de aplicaciones. 
El proveedor de nube controla la administración de la plataforma.

SaaS
Los usuarios pagan por el software que utilizan en un modelo de suscripción.
Modelo de precio de pago por uso.


## ¿Qué es la informática sin servidor?
Igual que PaaS, la informática sin servidor permite que los desarrolladores creen aplicaciones más rápidamente, ya que elimina la necesidad de administrar la infraestructura. En las aplicaciones sin servidor, el proveedor de servicios en la nube aprovisiona, escala y administra automáticamente la infraestructura necesaria para ejecutar el código. Las arquitecturas sin servidor son muy escalables y controladas por eventos, y solo usan recursos cuando se produce una función o un desencadenador concretos.

Es importante tener en cuenta que los servidores siguen ejecutando el código. El término "sin servidor" procede del hecho de que las tareas asociadas a la administración y el aprovisionamiento de la infraestructura son invisibles para el desarrollador. Este enfoque permite a los desarrolladores centrar su atención en la lógica de negocios y ofrecer más valor al núcleo de la empresa. La informática sin servidor ayuda a los equipos a aumentar su productividad y a llevar los productos al mercado con más rapidez, y permite a las organizaciones optimizar mejor los recursos y seguir centrándose en la innovación.
