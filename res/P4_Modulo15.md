# Parte 4 Modulo 5

##¿Qué es la defensa en profundidad?

El objetivo de la defensa en profundidad es proteger la información y evitar que personas no autorizadas a acceder a ella puedan sustraerla.
Una estrategia de defensa en profundidad usa una serie de mecanismos para ralentizar el avance de un ataque dirigido a adquirir acceso no autorizado a los datos.

## Capas de la defensa en profundidad
La defensa en profundidad se puede visualizar como un conjunto de capas, con los datos que se deben proteger en el centro.
![image](https://user-images.githubusercontent.com/86896526/126412839-c8932cc5-e549-4bfe-948b-0cb5317ba9ec.png)

Cada capa proporciona protección de modo que, si se produce una brecha en una capa, ya existe otra en funcionamiento para evitar una mayor exposición. Este enfoque elimina la dependencia de cualquier capa de protección única. Ralentiza un ataque y proporciona telemetría de alertas sobre la que pueden actuar los equipos de seguridad, ya sea de forma automática o manual.

- La capa de seguridad física es la primera línea de defensa para proteger el hardware informático del centro de datos.
  * La protección física del acceso a los edificios y el control del acceso al hardware de proceso del centro de datos son la primera línea de defensa.
  * La intención de la seguridad física es proporcionar medidas de seguridad físicas contra el acceso a los recursos. Estas medidas garantizan que no se puedan omitir otras capas y se controle apropiadamente la pérdida o el robo.

- La capa de identidad y acceso controla el acceso a la infraestructura y al control de cambios.
  * La capa de identidad y acceso consiste en garantizar que las identidades están protegidas, que solo se otorga el acceso necesario y que se registran los cambios y los eventos de inicio de sesión.
  En esta capa, es importante que realice lo siguiente:
  - * Controle el acceso a la infraestructura y al control de cambios.
  - * Use el inicio de sesión único (SSO)y la autenticación multifactor.
  - * Audite los eventos y los cambios.
  
- La capa perimetral usa protección frente a ataques de denegación de servicio distribuido (DDoS) para filtrar los ataques a gran escala antes de que puedan causar una denegación de servicio para los usuarios.
    * En el perímetro de la red, se trata de la protección frente a ataques basados en red contra los recursos. Identificar estos ataques, eliminar sus repercusiones y recibir alertas sobre ellos cuando suceden son formas importantes de proteger la red.
    En esta capa, es importante que realice lo siguiente:
  - * Use protección contra DDoS para filtrar los ataques a gran escala antes de que puedan afectar a la disponibilidad de un sistema para los usuarios.
  - * Use firewalls perimetrales para identificar los ataques malintencionados contra la red y alertar sobre ellos.

- La capa de red limita la comunicación entre los recursos a través de controles de acceso y segmentación.
  * En esta capa, el enfoque está en limitar la conectividad de la red en todos los recursos para permitir solo la necesaria. Al limitar esta comunicación, se reduce el riesgo de que se propaguen los ataques a otros sistemas de la red.
   En esta capa, es importante que realice lo siguiente:
  - * Limite la comunicación entre los recursos.
  - * Deniegue de forma predeterminada.
  - * Restrinja el acceso entrante de Internet y limite el saliente cuando sea apropiado.
  - * Implemente conectividad segura a las redes locales.

- La capa de proceso protege el acceso a las máquinas virtuales.
  * El software malintencionado, los sistemas sin revisiones aplicadas y los sistemas protegidos inadecuadamente abren el entorno a los ataques. El enfoque en esta capa es asegurarse de que sus recursos de proceso estén seguros y de que cuenta con los controles adecuados para minimizar los problemas de seguridad.
  En esta capa, es importante que realice lo siguiente:
  - * Proteja el acceso a las máquinas virtuales.
  - * Implemente la protección del punto de conexión de los dispositivos y mantenga los sistemas revisados y actualizados.



- La capa de aplicación ayuda a garantizar que las aplicaciones sean seguras y estén libres de vulnerabilidades de seguridad.
  * La integración de la seguridad en el ciclo de vida de desarrollo de aplicaciones ayuda a reducir el número de vulnerabilidades en el código. Todos los equipos de desarrollo deberían asegurarse de que sus aplicaciones son seguras de forma predeterminada.
  
  En esta capa, es importante que realice lo siguiente:
  - * Garantice que las aplicaciones son seguras y están libres de vulnerabilidades.
  - * Almacene los secretos de aplicación confidenciales en un medio de almacenamiento seguro.
  - * Convierta la seguridad en un requisito de diseño en todo el desarrollo de aplicaciones.

- La capa de datos controla el acceso a los datos empresariales y de clientes que es necesario proteger.

 * Los que almacenan y controlan el acceso a los datos son responsables de asegurarse de que están protegidos correctamente. A menudo, los requisitos legales dictan los controles y procesos que deben cumplirse para garantizar la confidencialidad, la integridad y la disponibilidad de los datos.
    
    En casi todos los casos, los atacantes intentan conseguir datos:
  - * Almacenados en una base de datos.
  - * Almacenados en discos en máquinas virtuales.
  - * Almacenados en aplicaciones de software como servicio (SaaS), como Office 365.
  - * Administrados mediante el almacenamiento en la nube.

## Posición de seguridad

El nivel de seguridad es la capacidad de su organización de protegerse frente a amenazas de seguridad y responder a ellas. Los principios comunes usados para definir un nivel de seguridad son la confidencialidad, la integridad y la disponibilidad, lo que se conoce colectivamente como CIA por sus siglas en inglés.

### Confidencialidad

El principio de privilegios mínimos implica restringir el acceso a la información únicamente a los usuarios a las que se concede acceso de forma explícita, solo al nivel necesario para realizar su trabajo. Esta información incluye la protección de contraseñas de usuario, contenido de correo electrónico y niveles de acceso a las aplicaciones y a la infraestructura subyacente.

### Integridad

Evitar cambios no autorizados en la información:

En reposo: cuando se almacenan.
En tránsito: cuando se transfieren de un lugar a otro, incluido desde un equipo local a la nube.
Un enfoque común que se usa en la transmisión de datos es la creación de una huella digital única de los datos por parte del remitente mediante un algoritmo hash unidireccional. El hash se envía al receptor junto con los datos. El receptor vuelve a calcular el hash de los datos y lo compara con el original para asegurarse de que los datos no se han perdido ni modificado en tránsito.

### Disponibilidad

Asegúrese de que los servicios funcionan y que solo pueden acceder a ellos los usuarios autorizados. Los ataques por denegación de servicio están diseñados para degradar la disponibilidad de un sistema, lo que afecta a sus usuarios.
