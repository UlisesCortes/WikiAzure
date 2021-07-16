# Parte 4 Modulo 14

# Protección frente a amenazas de seguridad en Azure

## Azure Security Center
Azure Security Center es un servicio de supervisión que proporciona visibilidad del nivel de seguridad en todos los servicios, tanto en Azure como en el entorno local. El término nivel de seguridad se refiere a las directivas y a los controles de ciberseguridad, así como a la predicción, la prevención y la respuesta a las amenazas de seguridad.

Security Center puede:

- Supervisar la configuración de seguridad en las cargas de trabajo locales y en la nube.
- Aplicar automáticamente la configuración de seguridad necesaria a los nuevos recursos a medida que se publican en línea.
- Proporcionar recomendaciones de seguridad basadas en las configuraciones, los recursos y las redes actuales.
- Supervisar de forma continua los recursos y realizar valoraciones de seguridad automáticas para identificar posibles vulnerabilidades antes de que alguien las aproveche.
- Usar el aprendizaje automático para detectar y bloquear la instalación de malware en las máquinas virtuales (VM) y otros recursos. También puede usar controles de aplicaciones adaptables para definir reglas que indiquen las aplicaciones permitidas a fin de garantizar que solo se puedan ejecutar las aplicaciones permitidas.
- Detectar y analizar posibles ataques entrantes e investigar amenazas y otras actividades posteriores a una brecha que pudieran haberse producido.
- Proporcionar control de acceso Just-in-Time a los puertos de red. Esto reduce la superficie expuesta a ataques al garantizar que la red solo permite el tráfico necesario en el momento en que se necesita.

### ¿Qué es la puntuación de seguridad?
La puntuación de seguridad es una medida del nivel de seguridad de una organización.

La puntuación de seguridad se basa en controles de seguridad, o en grupos de recomendaciones de seguridad relacionadas. La puntuación se basa en el porcentaje de controles de seguridad que se satisfacen. Cuantos más controles de seguridad se satisfacen, mayor es la puntuación que se recibe. La puntuación mejora cuando se corrigen todas las recomendaciones de un único recurso dentro de un control.

El seguimiento de las recomendaciones de la puntuación de seguridad ayuda a proteger a la organización frente a amenazas. Desde un panel centralizado de Azure Security Center, las organizaciones pueden supervisar la seguridad de sus recursos de Azure, como identidades, datos, aplicaciones, dispositivos e infraestructura, y trabajar en ella.

La puntuación de seguridad ayuda a:

- Notificar el estado actual del nivel de seguridad de la organización.
- Mejorar el nivel de seguridad al proporcionar detectabilidad, visibilidad, orientación y control.
- Comparar con los puntos de referencia y establecer indicadores clave de rendimiento (KPI).


### Protección frente a amenazas

- Acceso de máquina virtual Just-In-Time
Tailwind Traders configurará el acceso Just-in-Time a las máquinas virtuales. Este acceso bloquea el tráfico de forma predeterminada en puertos de red específicos de máquinas virtuales, pero permite el tráfico durante un tiempo especificado cuando un administrador lo solicita y lo aprueba.

- Controles de aplicación adaptables
Tailwind Traders puede controlar qué aplicaciones se pueden ejecutar en sus máquinas virtuales. En segundo plano, Security Center usa aprendizaje automático para examinar los procesos que se ejecutan en una máquina virtual. Crea reglas de excepción para cada grupo de recursos que contiene las máquinas virtuales y proporciona recomendaciones. Este proceso proporciona alertas que notifican a la empresa si hay aplicaciones no autorizadas en ejecución en sus máquinas virtuales.

- Protección de red adaptable
Security Center puede supervisar los patrones de tráfico de Internet de las máquinas virtuales y compararlos con la configuración actual de los grupos de seguridad de red (NSG) de la empresa. A partir de ahí, Security Center puede hacer recomendaciones sobre si los NSG deben bloquearse más y proporcionar pasos de corrección.

- Supervisión de la integridad de los archivos
Tailwind Traders también puede configurar la supervisión de los cambios en archivos importantes tanto en Windows como en Linux, la configuración del registro, las aplicaciones y otros aspectos que podrían indicar un ataque de seguridad.

### Responder a alertas de seguridad

## Detección de amenazas de seguridad y respuesta a ellas mediante Azure Sentinel
 ## Azure Sentinel

Azure Sentinel es el sistema SIEM basado en la nube de Microsoft. Usa análisis de seguridad inteligente y análisis de amenazas.

### Capacidades de Azure Sentinel
  - Recopilar datos en la nube a gran escala
  - Detectar amenazas no detectadas anteriormente
  - Investigar amenazas con inteligencia artificial
  - Responder a incidentes rápidamente

### Conexión de los orígenes de datos

Azure Sentinel admite una serie de orígenes de datos que puede analizar en busca de eventos de seguridad. Estas conexiones las administran conectores integrados o API y formatos de registro estándar del sector.

- Conexión de soluciones de Microsoft
Los conectores proporcionan integración en tiempo real para servicios como las soluciones de Protección contra amenazas de Microsoft, orígenes de Microsoft 365 (incluido Office 365), Azure Active Directory y Firewall de Windows Defender.

- Conexión con otros servicios y soluciones
Hay conectores disponibles para servicios y soluciones comunes que no son de Microsoft, incluidos AWS CloudTrail, Citrix Analytics (Security), Sophos XG Firewall, VMware Carbon Black Cloud y Okta SSO.

- Conexión con orígenes de datos estándar del sector
Azure Sentinel admite datos de otros orígenes que usan el estándar de mensajería Formato de evento común (CEF), Syslog o la API REST.

### Detectar amenazas

Los análisis integrados usan plantillas diseñadas por el equipo de expertos y analistas de seguridad de Microsoft que se basan en amenazas conocidas, vectores de ataque comunes y cadenas de escalado de actividades sospechosas. Estas plantillas se pueden personalizar y buscan cualquier actividad que parezca sospechosa en el entorno. En algunas plantillas se usan análisis de comportamiento de aprendizaje automático que se basan en algoritmos propiedad de Microsoft.

Los análisis personalizados son reglas que se crean para buscar criterios concretos en el entorno. Se puede obtener una vista previa del número de resultados que generaría la consulta (en función de eventos de registro pasados) y establecer una programación para que se ejecute la consulta. También se puede establecer un umbral de alerta.

## Almacenamiento y administración de secretos mediante Azure Key Vault
## Azure Key Vault
Azure Key Vault es un servicio en la nube centralizado para almacenar los secretos de la aplicación en una única ubicación central. Proporciona un acceso seguro a la información confidencial mediante capacidades de control de acceso y registro.

- Administración de secretos
Puede usar Key Vault para almacenar de forma segura y controlar exhaustivamente el acceso a tokens, contraseñas, certificados, claves de API y otros secretos.

- Administrar claves de cifrado
Puede usar Key Vault como solución de administración de claves. Key Vault facilita la creación y el control de las claves de cifrado que se emplean para cifrar los datos.

- Administrar certificados SSL/TLS
Key Vault permite aprovisionar, administrar e implementar los certificados públicos y privados de Capa de sockets seguros/Seguridad de la capa de transporte (SSL/TLS) de los recursos de Azure y los recursos internos.

- Almacenar secretos respaldados por módulos de seguridad de hardware (HSM)
Estas claves y secretos se pueden proteger mediante software o mediante HSM validados por FIPS 140-2 nivel 2.

### ¿Cuáles son las ventajas de Azure Key Vault?
Las ventajas del uso de Key Vault incluyen:

- Secretos de aplicación centralizados
La centralización del almacenamiento de los secretos de la aplicación permite controlar su distribución y reduce las posibilidades de que se filtren accidentalmente.

- Secretos y claves almacenados de forma segura
Azure usa algoritmos estándar del sector, longitudes de clave y HSM. El acceso a Key Vault requiere una autenticación y autorización adecuadas.

- Supervisión y control de acceso
Con Key Vault, puede supervisar y controlar el acceso a los secretos de la aplicación.

- Administración simplificada de secretos de aplicación
Key Vault facilita la inscripción y la renovación de certificados de entidades de certificación (CA) públicas. También puede escalar verticalmente y replicar contenido dentro de las regiones y usar herramientas de administración de certificados estándar.

- Integración con otros servicios de Azure
Puede integrar Key Vault con cuentas de almacenamiento, registros de contenedor, centros de eventos y muchos más servicios de Azure. Después, estos servicios pueden hacer referencia de forma segura a los secretos almacenados en Key Vault.

# Ejercicio

# Hospedaje de máquinas virtuales de Azure en servidores físicos dedicados mediante Azure Dedicated Host
 # Azure Dedicated Host
Azure Dedicated Host proporciona servidores físicos dedicados para hospedar las máquinas virtuales de Azure para Windows y Linux.

Azure Dedicated Host:

- Ofrece visibilidad y control sobre la infraestructura de servidor que ejecuta las máquinas virtuales de Azure.
- Ayuda a satisfacer requisitos de cumplimiento mediante la implementación de las cargas de trabajo en un servidor aislado.
- Permite elegir el número de procesadores, capacidades de servidor, series de máquinas virtuales y tamaños de máquina virtual dentro del mismo host.

### Concideraciones de dsiponibilidad
Para lograr una alta disponibilidad, puede aprovisionar varios hosts en un grupo host e implementar las máquinas virtuales en este grupo. Las máquinas virtuales en hosts dedicados también pueden aprovechar las ventajas del control de mantenimiento. Esta característica permite controlar cuándo se producen las actualizaciones de mantenimiento regulares, dentro de una ventana gradual de 35 días.

### Consideraciones sobre precios
Se cobra por host dedicado, con independencia de cuántas máquinas virtuales se implementen en él. El precio del host se basa en la familia de máquinas virtuales, el tipo (tamaño de hardware) y la región.

![image](https://user-images.githubusercontent.com/86896526/125994501-3d5e6382-d0cb-4a49-a43f-8c4a4e54bc8d.png)
![image](https://user-images.githubusercontent.com/86896526/125994410-7221d7dd-865d-411a-bd90-d44bc75c684a.png)
![image](https://user-images.githubusercontent.com/86896526/125994431-cfebdbd9-6b97-44dd-9184-6a6048ddd44f.png)
![image](https://user-images.githubusercontent.com/86896526/125994389-2d9fc46a-ae56-4e81-af90-014647c3e47c.png)

Ejercicio


