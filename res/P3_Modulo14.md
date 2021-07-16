# Parte 3 Modulo 14
# Elección del mejor servicio de supervisión para visibilidad, información y mitigación de interrupciones.

Los sistemas de software modernos que se ejecutan en la nube son complejos, por lo que conocer el estado y el rendimiento de su entorno de hospedaje de aplicaciones —con todos sus niveles de servicios— supone todo un reto.

## Identificación de las opciones de productosIdentificación de las opciones de productos
Opciones de productos
A nivel general, hay tres ofertas principales de supervisión de Azure, cada una de las cuales tiene como objetivo una audiencia y un caso de uso específicos, y proporcionan un conjunto diverso de herramientas, servicios, API de programación, etc.

### Azure Advisor
### Quiere recibir una alerta cuando haya disponibles nuevas recomendaciones para mejorar su entorno de nube. ¿Qué servicio puede hacer esto?
Azure Advisor evalúa los recursos de Azure y hace recomendaciones que contribuyen a mejorar la confiabilidad, la seguridad y el rendimiento, lograr la excelencia operativa y reducir los costos. Advisor está diseñado para ayudarle a ahorrar tiempo en la optimización en la nube. El servicio de recomendaciones sugiere medidas que puede adoptar de inmediato, posponer o descartar.

Las recomendaciones están disponibles con Azure Portal y la API. Además, es posible configurar notificaciones para estar al tanto de las nuevas recomendaciones.

El panel Advisor de Azure Portal muestra recomendaciones personalizadas para todas las suscripciones, y los filtros permiten seleccionar recomendaciones para suscripciones, grupos de recursos o servicios específicos. Las recomendaciones se dividen en cinco categorías:

- Confiabilidad: se usa para garantizar y mejorar la continuidad de las aplicaciones críticas para la empresa.
- Seguridad: se usa para detectar amenazas y vulnerabilidades que podrían dar lugar a infracciones de seguridad.
- Rendimiento: se usa para mejorar la velocidad de las aplicaciones.
- Costos: se usan para optimizar y reducir el gasto general de Azure.
- Excelencia operativa: se usa para conseguir procedimientos recomendados de eficiencia en procesos y flujos de trabajo, manejabilidad de los recursos e implementación.

### ¿Necesita analizar cómo usa Azure para reducir los costos? ¿Mejorar la resistencia? ¿Fortalecer la seguridad?
Elija Azure Advisor si quiere realizar un análisis de los recursos implementados. Azure Advisor analiza la configuración y el uso de los recursos, y ofrece sugerencias sobre cómo optimizar la confiabilidad, la seguridad, el rendimiento, los costos y las operaciones según los procedimientos recomendados por los expertos.

### Azure Monitor
### ¿Qué servicio es una plataforma en la que se basa Application Insights y permite la supervisión de máquinas virtuales, contenedores y Kubernetes?
Azure Monitor es una plataforma que permite recopilar, analizar y mostrar datos, así como llevar a cabo acciones en función de las métricas y los datos registrados en todo el entorno local y de Azure.

El diagrama siguiente muestra lo completo que es Azure Monitor.
![image](https://user-images.githubusercontent.com/86896526/125987610-d76afefd-a666-4882-838b-f20f808e4362.png)

- A la izquierda aparece una lista de los orígenes de los datos de métricas y registros, que pueden recopilarse en cada nivel de la arquitectura de aplicaciones, desde la aplicación hasta el sistema operativo y la red.

- En el centro, puede ver cómo se almacenan los datos de registro y métricas en los repositorios centrales.

- A la derecha, los datos se usan de diversas formas. Puede ver el rendimiento histórico y en tiempo real de cada nivel de la arquitectura, o bien consultar información combinada y detallada. Los datos se muestran en diferentes niveles para distintas audiencias. Puede ver informes de alto nivel en el panel de Azure Monitor o crear vistas personalizadas mediante consultas de Power BI y Kusto.

Además, puede usar los datos para ayudarle a reaccionar ante eventos críticos en tiempo real gracias a las alertas enviadas a los equipos por SMS, correo electrónico, etc. También hay la opción de usar umbrales que, en caso de aumento o disminución de la demanda, desencadenen la funcionalidad de escalado automático.

### ¿Necesita configurar alertas para las interrupciones o para cuando el escalado automático está a punto de implementar nuevas instancias?
### ¿Quiere medir eventos personalizados junto con otras métricas de uso?
Elija Azure Monitor si quiere medir eventos personalizados y otros datos de telemetría recopilados. Los eventos personalizados, como los agregados al código fuente de las aplicaciones de software, pueden ayudar a identificar y diagnosticar la razón por la que la aplicación se comporta de una manera determinada.

### Azure Service Health
### ¿Qué servicio ofrece un análisis oficial de la causa principal (RCA) de la interrupción en los incidentes de Azure?
Azure Service Health proporciona una vista personalizada del estado de los servicios, regiones y recursos de Azure en los que se basa su infraestructura. El sitio web status.azure.com, que muestra solo los principales problemas que afectan de manera generalizada a los clientes de Azure, no refleja el panorama completo. Sin embargo, Azure Service Health muestra los problemas detectados de mayor y menor importancia que le afectan. Los problemas del servicio son poco frecuentes, pero es importante estar preparado para lo inesperado. Por ello, puede configurar alertas que le ayuden a evaluar las interrupciones y el mantenimiento planeado. Después de una interrupción, Service Health proporciona informes de incidentes oficiales, llamados análisis de la causa principal (RCA), que puede compartir con las partes interesadas.

Service Health le ayuda a supervisar varios tipos de eventos:

- Los problemas de servicio son problemas de Azure, como las interrupciones, que le afectan en este momento. Puede profundizar en los servicios y las regiones afectados, así como en las actualizaciones de los equipos de ingeniería, a fin de encontrar la manera de compartir la información más reciente y realizar un seguimiento de esta.

- Mantenimiento planeado: este tipo de eventos pueden afectar a la disponibilidad. Puede profundizar en los servicios, las regiones y los detalles afectados para mostrar cómo influirá un evento y qué debe hacer. La mayoría de estos eventos se producen sin que tengan ningún impacto en el usuario y no se mostrarán aquí. En el caso excepcional de que se requiera un reinicio, Service Health le permitirá elegir cuándo realizar el mantenimiento para minimizar el tiempo de inactividad.

- Avisos de estado: son problemas que exigen actuar para evitar la interrupción del servicio, e incluyen retiradas del servicio y cambios importantes. Los avisos de estado se anuncian con mucha antelación para que pueda planear su respuesta.

### ¿Quiere supervisar los servicios de Azure o el uso de Azure?
Si quiere mantener un control de Azure, especialmente de los servicios y regiones de los que dependa, debe elegir Azure Service Health. Puede ver el estado actual de los servicios de Azure de los que depende, las próximas interrupciones planeadas y los próximos servicios que se lanzarán. Puede configurar alertas que le permitan estar al día de incidentes y tiempos de inactividad futuros sin tener que visitar el panel con regularidad.
