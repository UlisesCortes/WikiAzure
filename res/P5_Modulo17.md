# Parte 5 Modulo 17
Creación de una estrategia de gobernanza en la nube en Azure

#  Gobernanza 
Describe el proceso general por el que se establecen reglas y directivas y se garantiza que esas reglas y directivas se aplican.

# Cloud Adoption Framework para Azure
Sirve como guía consolidada para ayudar en el recorrido para la adopción de la nube. Cloud Adoption Framework ayuda a crear e implementar las estrategias empresariales y tecnológicas necesarias para usar la nube correctamente.

## Qué se incluye en Cloud Adoption Framework
 Cloud Adoption Framework incluye estas fases:

* Definir la estrategia.
* Crear un plan.
* Preparar la organización.
* Adoptar la nube.
* Controlar y administrar los entornos de nube.

![image](https://user-images.githubusercontent.com/86896526/126708938-7089d7a9-8d7f-494a-baa4-55ccae6b21bb.png)

La fase de control se centra en la gobernanza en la nube. Cloud Adoption Framework se puede consultar como referencia para obtener instrucciones recomendadas mientras traza su estrategia de gobernanza en la nube.

# Sobre el Cloud Adoption Framework

<!-- TOC -->
- [Sobre el Cloud Adoption Framework](#sobre-el-cloud-adoption-framework)
  - [1 Definir la estrategia.](#1-definir-la-estrategia)
    - [1.1 Definir y documentar las motivaciones](#11-definir-y-documentar-las-motivaciones)
    - [1.2 Documentación de los resultados empresariales](#12-documentación-de-los-resultados-empresariales)
    - [1.3 Desarrollo de un caso empresarial](#13-desarrollo-de-un-caso-empresarial)
    - [1.4 Elección adecuada del primer proyecto](#14-elección-adecuada-del-primer-proyecto)
  - [2 Creación del plan](#2-creación-del-plan)
    - [2.1 Patrimonio digital](#21-patrimonio-digital)
    - [2.2 Alineación inicial de la organización](#22-alineación-inicial-de-la-organización)
    - [2.3 Plan de preparación de las aptitudes](#23-plan-de-preparación-de-las-aptitudes)
    - [2.4 Plan de adopción de la nube](#24-plan-de-adopción-de-la-nube)
  - [3 Preparación de la organización](#3-preparación-de-la-organización)
    - [3.1 Guía de instalación de Azure](#31-guía-de-instalación-de-azure)
    - [3.2 Zonas de aterrizaje de Azure](#32-zonas-de-aterrizaje-de-azure)
    - [3.3 Expansión de la zona de aterrizaje](#33-expansión-de-la-zona-de-aterrizaje)
    - [3.4 Procedimientos recomendados](#34-procedimientos-recomendados)
  - [4 Adopción de la nube - Fase de migración](#4-adopción-de-la-nube---fase-de-migración)
    - [4.1 Migración de la primera carga de trabajo](#41-migración-de-la-primera-carga-de-trabajo)
    - [4.2 Escenarios de migración](#42-escenarios-de-migración)
    - [4.3 Procedimientos recomendados](#43-procedimientos-recomendados)
    - [4.4 Mejoras de proceso](#44-mejoras-de-proceso)
      - [Previsión de un estado final](#previsión-de-un-estado-final)
      - [Migración incremental](#migración-incremental)
  - [4 Adopción de la nube - Fase de innovación](#4-adopción-de-la-nube---fase-de-innovación)
    - [4.1 Consenso del valor empresarial](#41-consenso-del-valor-empresarial)
    - [4.2 Guía de innovación de Azure](#42-guía-de-innovación-de-azure)
    - [4.3 Procedimientos recomendados](#43-procedimientos-recomendados-1)
    - [4.4 Bucles de comentarios](#44-bucles-de-comentarios)
  - [5 Control y administración de los entornos de nube](#5-control-y-administración-de-los-entornos-de-nube)
    - [Gobernanza](#gobernanza)
      - [5.1 Metodología](#51-metodología)
        - [Previsión de un estado final](#previsión-de-un-estado-final-1)
        - [Alcanzar el estado final](#alcanzar-el-estado-final)
      - [5.2 Banco de pruebas](#52-banco-de-pruebas)
      - [5.3 Base de gobernanza inicial](#53-base-de-gobernanza-inicial)
      - [5.4 Mejora de la base de gobernanza inicial](#54-mejora-de-la-base-de-gobernanza-inicial)
    - [Administración](#administración)
      - [5.1 Definición de los compromisos empresariales](#51-definición-de-los-compromisos-empresariales)
      - [5.2 Establecimiento de una base de referencia de administración](#52-establecimiento-de-una-base-de-referencia-de-administración)
        - [Guía de administración de Azure: Antes de comenzar](#guía-de-administración-de-azure-antes-de-comenzar)
      - [5.3 Expansión de la base de referencia de administración](#53-expansión-de-la-base-de-referencia-de-administración)
        - [Procedimientos recomendados viables](#procedimientos-recomendados-viables)
      - [5.4 Operaciones avanzadas y principios de diseño](#54-operaciones-avanzadas-y-principios-de-diseño)
  - [Recursos adicionales](#recursos-adicionales)

<!-- /TOC -->

El Cloud Adoption Framework es una guía que sirve para el recorrido de la implementación de tecnologías de nube en una organización. 

Este marco de trabajo contempla tareas organizacionales, técnicas y de planeación para la correcta migración a la nube.

**Aquí te mostraré los pasos a base de ejemplos, pasos a seguir o entregables posibles.**

- [Descarga aquí todas las plantillas de documentación adaptadas a Microsoft Azure](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/reference/tools-templates)

## 1 Definir la estrategia.

[Template sugerido para esta etapa](/res/docs/cloud-adoption-framework-strategy-and-plan-template.docx)

### 1.1 Definir y documentar las motivaciones

:book: Reúnase con las partes interesadas clave y la dirección para documentar la motivación que hay detrás de la adopción de la nube.

Algunas posibles motivaciones para migrar a la nube son:
- Ahorros en costos
- Reducción de la complejidad técnica o de proveedores
- Optimización de las operaciones internas
- Aumento de agilidad empresarial
- Preparación para nuevas funcionalidades técnicas
- Escalado para satisfacer demandas del mercado
- Escalado para satisfacer demandas geográficas
- Integración de una cartera de TI compleja

Sin embargo, la organización se puede centrar más en la innovacción como con los siguientes ejemplos:
- Aumento de la agilidad comercial
- Preparación para nuevas funcionalidades técnicas
- Creación de nuevas funcionalidades técnicas
- Escalado para satisfacer demandas del mercado
- Escalado para satisfacer demandas geográficas
- Experiencias de los clientes mejoradas e involucración
- Transformación de productos o servicios

### 1.2 Documentación de los resultados empresariales

:book: Implique a las partes interesadas y a los ejecutivos motivados para que documenten resultados empresariales concretos.

[Plantilla de resultados empresariales](/res/docs/business-outcome-template.xlsx)

Algunos de los resultados emrpesariales esperados por digferenets roles son:

- **Liderazgo financiero**: aumentar la rentabilidad sin perder de vista el cumplimiento
- **Marketing**: lograr nuevos clientes, conservar los conseguidos y crear una reputación
- **Ventas**: acelerar las ventas, mejorar el valor de los clientes
- **Recursos humanos**: conservar, contratar y capacitar a los empleados
- **Liderazgo ejecutivo**: cumplir los requisitos de crecimiento del mercado y las métricas de sostenibilidad medioambiental

Cada rol puede generar entregables y resultados diferentes. Por ejemplo, los resultados fiscales pueden ser las declaraciones de impuestos, proyecciones de ventas, presupuestos, etc.

### 1.3 Desarrollo de un caso empresarial

:book: Desarrolle un caso de negocio para validar el modelo financiero que sea compatible con las motivaciones y los resultados.

Las migraciones a la nube pueden generar una rápida rentabilidad de la inversión (ROI) por los esfuerzos de transformación en la nube.

![ROI](/res/images/roi.jpg)

El ROI puede ser una buena justificación para una migración a la nube ya que determina que cantidad de ingresos y tiempo necesitas para recuperar la inversión hecha.

El costo o inversión inicial puede contemplar:
- Capacitación del equipo
- Costos de la migración
- Costo por tiempo invertido
- Inversión inicial en la nube. Consulta la [calculadora de precios de Azure](https://azure.microsoft.com/es-mx/pricing/calculator/)
  - Diferencia el costo contra un ambiente on-premise con [la calculadora de TCO](https://azure.microsoft.com/es-mx/pricing/tco/calculator/)

### 1.4 Elección adecuada del primer proyecto

:book: El primer proyecto de adopción de la nube le ayudará a alinear las motivaciones con los esfuerzos técnicos. Este artículo puede ayudarle a elegir el primer proyecto de un modo prudente.

Algunos rubros para elegir el proyecto pionero son:

- **Eventos empresariales críticos**: cuando un evento empresarial crítico es la motivación principal, la implementación de una herramienta como Azure Site Recovery podría ser un buen primer proyecto. Durante la migración, usarás una herramienta como Azure Migrate para migrar rápidamente los recursos del centro de datos. Pero durante el primer proyecto, podrás usar primero Azure Site Recovery como herramienta de recuperación ante desastres. Reduzce las dependencias en los recursos de recuperación ante desastres del centro de datos antes de planear pragmáticamente la migración.

- **Motivaciones de migración**: cuando la migración es la motivación principal, es aconsejable empezar con la migración de una carga de trabajo no crítica. En la guía de configuración de Azure y la guía de migración a Azure se proporcionan instrucciones para la migración de la primera carga de trabajo.

- **Motivaciones de innovación**: cuando la innovación es la motivación principal, la creación de un entorno de desarrollo y pruebas de destino puede ser un excelente primer proyecto.

También puedes empezar con proyectos como:
- No productivos o que no estén en ambientes de producción
- Interfaz de escritorio virtual (VDI)
- Desarrollo y pruebas
- Aplicaciones sencillas
- Laboratorios de pruebas

## 2 Creación del plan

### 2.1 Patrimonio digital

:book: Realiza el inventario y racionalización del patrimonio digital según supuestos que se alinean con las motivaciones y resultados empresariales.

1. Requieres de un **inventario** donde contemples completamente los recursos, aplicaciones, software, hardware, sistemas operativos y métricas de rendimiento del sistema.

2. Requieres hacer un **análisis cuantitativo** contestando preguntas como:

- ¿Está el recurso en uso hoy en día?
- Si es así, ¿está optimizado y dimensionado correctamente?
- ¿Qué dependencias existen entre los recursos?

3. **Análisis cualitativo** [Elige un enfoque de los presentados en este documento](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/digital-estate/approach)

4. **Decisión de racionalización** Usando los tres puntos anteriores, se toma la desición de Rehospedar, Refactorizar, Rediseñar, Volver a generar (Regenerate) o Remplazar los recursos. [Más información de las 5Rs de la racionalización aquí.](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/digital-estate/5-rs-of-rationalization#the-five-rs-of-rationalization)

### 2.2 Alineación inicial de la organización

:book: Establece un plan para la alineación inicial de la organización que admita el plan de adopción.

En este punto se asignan los recursos humanos y no humanos a las diferentes tareas que tendrá la organización de la nube. Por ejemplo:

- ¿Qué persona completará las tareas técnicas del plan de adopción de la nube?
- ¿Qué persona será responsable de la capacidad del equipo para entregar cambios técnicos?
- ¿Qué persona se encargará de la gobernanza?
- ¿Existen otras funcionalidades o personas que tengan responsabilidad en el plan de adopción de la nube?

### 2.3 Plan de preparación de las aptitudes

:book: Crea un plan para afrontar las carencias en la preparación de las aptitudes.

Para crear este plan necesitas:

1. Detectar y documentar las preocupaciones de cada equipo al adoptar la nube

Por ejemplo, el equipo de TI puede tener preocupaciones por el incremento en su necesidad de capacitación y ahí se incluirían las preferencias de entrenamiento en el plan de preparación.

2. Detección de brechas. Una brecha es un rol, aptitud o proceso necesario para la transformación digital que no existe actualmente en la empresa.

3. Trabajo en equipo interdisciplinario. Por ejemplo, tecnología con recursos humanos. 

### 2.4 Plan de adopción de la nube

:book: Desarrolla un plan de adopción de la nube para administrar los cambios en el patrimonio digital, las aptitudes y la organización.

1. **Requisitos previos**: confirma que se han completado todos los pasos de requisitos previos antes de crear el plan.

2. **Definición y clasificación por prioridades de las cargas de trabajo**: clasifiqua por prioridades las 10 primeras cargas de trabajo para establecer un trabajo pendiente de adopción inicial.

3. **Adaptación de los recursos a las cargas de trabajo**: identifica qué recursos (propuestos o existentes) son necesarios para posibilitar las cargas de trabajo clasificadas por prioridades.

4. **Revisión de las decisiones de racionalización**: revisa las decisiones de racionalización para refinar las decisiones de la ruta de adopción: **migrar o innovar**.

5. **Establecimiento de iteraciones y planes de versiones**: las iteraciones son los bloques de tiempo asignados para realizar el trabajo. Las versiones son la definición del trabajo que se debe realizar antes de desencadenar un cambio en los procesos de producción.

6. **Estimación del tiempo**: establece escalas de tiempo aproximadas para fines de planeamiento de versiones, en función de las estimaciones iniciales.

## 3 Preparación de la organización

### 3.1 Guía de instalación de Azure

:book: Revisa la guía de instalación de Azure para familiarizarse con las herramientas y los enfoques necesarios para crear una zona de aterrizaje.

- [Introducción a la guía de configuración de Azure](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/ready/azure-setup-guide/)

### 3.2 Zonas de aterrizaje de Azure

:book: Elige la opción de zona de aterrizaje más adecuada para establecer un punto de partida basado en código para su entorno.

Las zonas de aterrizaje de Azure permiten la migración de aplicaciones y el desarrollo. 

Es la puesta en marcha de varias suscripciones que tiene en cuenta la escala, seguridad, gobernanza, redes e identidad para poder comenzar a trabajar con la nube.

### 3.3 Expansión de la zona de aterrizaje

:book: Amplía la primera zona de aterrizaje para cumplir los requisitos de plataforma del plan de adopción de la nube.

- **Consideraciones básicas**: refactoriza una zona de aterrizaje para refinar el hospedaje, los fundamentos y otros elementos básicos.
- **Expansiones de operaciones**: agrega configuraciones de administración de operaciones para mejorar el rendimiento, la confiabilidad y la excelencia operativa.
- **Expansiones de gobernanza**: agrega configuraciones de la gobernanza para mejorar el costo, la confiabilidad, la seguridad y la coherencia.
- **Expansiones de seguridad**: agrega configuraciones de la seguridad para mejorar la protección de los datos confidenciales y los sistemas críticos.

### 3.4 Procedimientos recomendados

:book: Utiliza los procedimientos recomendados para validar las modificaciones de la zona de aterrizaje, con el fin de garantizar la correcta configuración de las zonas de aterrizaje actuales y futuras.

Estas recomendaciones dependerán de los recursos, el tipo de solución a implementar, las áreas, la organización...

## 4 Adopción de la nube - Fase de migración

### 4.1 Migración de la primera carga de trabajo

:book: usa la guía de migración de Azure para familiarizarte tanto con las herramientas nativas de Azure como con el método de migración.

- [Guía de migración a la nube](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/migrate/azure-migration-guide/?tabs=MigrationTools)

### 4.2 Escenarios de migración

:book: Usa otros enfoques y herramientas de migración para actuar en otros escenarios de migración.

- [Migración de acuerdo a las herramientas de origen](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/migrate/azure-best-practices/)

### 4.3 Procedimientos recomendados

:book: Aborda las necesidades comunes de migración mediante la aplicación de procedimientos recomendados coherentes.

- [Migración de acuerdo a las herramientas de origen](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/migrate/azure-best-practices/)

### 4.4 Mejoras de proceso

:book: La migración es una actividad de proceso intensivo. A medida que se escalan los esfuerzos de migración, utilice estas mejoras de procesos para evaluar y consolidar diversos aspectos de la migración.

- [5Rs de la racionalización](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/digital-estate/5-rs-of-rationalization#the-five-rs-of-rationalization)

La migración y modernización de las cargas de trabajo van desde simples migraciones de rehospedaje (llamadas también migraciones lift and shift) mediante las funcionalidades de infraestructura como servicio (IaaS) que no requieren cambios de código y aplicaciones, pasando por la refactorización con cambios mínimos, hasta el rediseño para modificar y ampliar la funcionalidad de código y aplicaciones para aprovechar las tecnologías de la nube.

#### Previsión de un estado final

Es importante tener una visión aproximada del estado final antes de iniciar los trabajos de migración.

![Migración estado final](/res/images/migration-options.png)

#### Migración incremental

El modelo de migración de Cloud Adoption Framework se basa en un proceso de transformación incremental en la nube. Asume que la organización comenzará con un esfuerzo inicial, de ámbito limitado, de migración a la nube, al que nos referimos comúnmente como la primera carga de trabajo. Este esfuerzo se ampliará de forma iterativa para incluir más cargas de trabajo a medida que los equipos de operaciones perfeccionen y mejoren sus procesos de migración.

![Migración incremental](/res/images/methodology-migrate-caf.png)

## 4 Adopción de la nube - Fase de innovación

![Innovate Methodology](/res/images/innovate-methodology.png)

### 4.1 Consenso del valor empresarial

:book: Antes de decidir qué soluciones técnicas vas a usar, identifica de qué forma la innovación puede potenciar el valor empresarial. Asigna ese valor a su estrategia en la nube. En esta metodología incremental, el valor empresarial se representa mediante una hipótesis acerca de las necesidades del cliente.

1. Preguntate primero:

- ¿Qué necesidad definida del cliente busca satisfacer con esta solución?
- ¿Qué oportunidades creará esta solución para la empresa?
- ¿Qué resultados empresariales se lograrán con esta solución?
- ¿Qué motivación de la empresa se atenderá con esta solución?

2. Observa primero la perspectiva general y las oportunidades
3. Solucionar la alineación de la solución. Para ello necesitas identificar:

- Oportunidad de hipótesis
- Oportunidad de creación
- Oportunidad de aprendizaje

### 4.2 Guía de innovación de Azure

Azure incluye herramientas en la nube que aceleran la implementación de soluciones innovadoras. En función de lo que necesitas, puede plantearse varias combinaciones de herramientas. Se recomienda crear un producto viable mínimo con herramientas básicas.

- [Introducción a la guía de soluciones innovadoras de Azure
](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/innovate/innovation-guide/)

### 4.3 Procedimientos recomendados

:book: Las decisiones arquitectónicas deberían seguir los procedimientos recomendados en todas las herramientas de la cadena. esta guía acelerará más el desarrollo de soluciones y proporcionará una referencia para la creación de diseños arquitectónicos sólidos.

![Innovaction Toolchain](/res/images/innovate-toolchain.png)


- **Democratización de datos**: herramientas para compartir datos que satisfagan las necesidades de los clientes relacionadas con la información.
- **Participación a través de aplicaciones**: Herramientas para crear aplicaciones que permitan la participación de los clientes más allá de los datos sin procesar.
- **Capacitación de la adopción**: herramientas para acelerar la adopción por parte del cliente mediante el apoyo digital a los ciclos de crear-medir-aprender.
- **Interacción con dispositivos**: herramientas para crear distintos niveles de experiencias ambientales para los clientes.
- **Predicción e influencia**: herramientas para el análisis predictivo y la integración de su salida en aplicaciones.

### 4.4 Bucles de comentarios

:book:  Durante cada iteración de desarrollo, las soluciones en desarrollo ofrecen a los equipos aprender la posibilidad de aprender al mismo tiempo que sus clientes. Los bucles de comentarios rápidos y precisos con sus clientes pueden ayudarte a probar, medir y aprender mejor, y, en última instancia, a reducir el tiempo de impacto en el mercado. 

![Bucles de comentarios](/res/images/bml-feedback-loop.png)

## 5 Control y administración de los entornos de nube

### Gobernanza

#### 5.1 Metodología

:book: Establece un reconocimiento básico de la metodología que promueve la gobernanza en la nube dentro de Cloud Adoption Framework para empezar a pensar en la solución de estado final.

##### Previsión de un estado final

![Gobernanza 1](/res/images/operational-transformation-govern-large.png)

:book:  La gobernanza incremental se basa en un pequeño conjunto de directivas corporativas, procesos y herramientas para establecer una base para la adopción y la gobernanza. Esta base se denomina producto viable mínimo (MVP) . Un MVP permite al equipo de gobernanza incorporar con rapidez la gobernanza en las implementaciones a lo largo del ciclo de vida de la adopción. Se puede establecer un MVP en cualquier punto durante el proceso de adopción de la nube. Es recomendable adoptar un MVP tan pronto como sea posible.

##### Alcanzar el estado final

![Gobenrarza 2](/res/images/incremental-governance-example.png)

#### 5.2 Banco de pruebas

:book: Evaluación del estado actual y futuro para establecer una visión a la hora de aplicar la plataforma.

- [Usa esta herramienta](https://cafbaseline.com/)

#### 5.3 Base de gobernanza inicial

:book: Comienza tu recorrido por la gobernanza con un pequeño conjunto de herramientas de gobernanza de fácil implementación. Esta base de gobernanza inicial se denomina producto viable mínimo (MVP).

- [Guía de gobernanza para empresas estándar](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/govern/guides/standard/)

:book: El Producto Minimo Viable o MVP es la versión tempranda de un producto o servicio que sirve para validar solo la funcionalidad o validez de una idea o implementación.

- :movie_camera: [MVP desde la vista del emprendimiento](https://youtu.be/LCrMWe09EQY)

#### 5.4 Mejora de la base de gobernanza inicial

:book: Durante la implementación del plan de adopción de la nube, agrega de manera iterativa los controles de gobernanza para afrontar riesgos tangibles a medida que avanza hacia el estado final.

- [Vectores de madurez](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/govern/foundation-improvements#maturity-vectors)

### Administración

![CAF Manage](/res/images/caf-manage.png)

#### 5.1 Definición de los compromisos empresariales

:book: Documenta las cargas de trabajo admitidas para establecer los compromisos operativos con la empresa y acordar las inversiones en administración de la nube para cada carga de trabajo.

- El primer paso para crear la alineación empresarial es garantizar la alineación de los términos.

#### 5.2 Establecimiento de una base de referencia de administración

:book: Define los grados de importancia, las herramientas de administración de la nube y los procesos necesarios para ofrecer tu compromiso mínimo con la administración de operaciones.

##### Guía de administración de Azure: Antes de comenzar

- **Inventario y visibilidad**: cree un inventario de recursos en varias nubes. Desarrolle la visibilidad del estado de ejecución de cada recurso
- **Cumplimiento operativo**: establezca controles y procesos para asegurarse de que todos los estados están configurados correctamente y de que se ejecutan en un entorno bien controlado
- **Protección y recuperación**: asegúrese de que todos los recursos administrados están protegidos y se pueden recuperar mediante las herramientas de administración de la línea de base
- **Opciones de línea de base mejorada**: evalúe las incorporaciones comunes a la línea de base que puedan satisfacer las necesidades empresariales
- **Operaciones de la plataforma**: amplíe la línea de base de administración con un catálogo de servicios bien definido y plataformas administradas centralmente
- **Operaciones con cargas de trabajo**: amplíe la línea de base de administración para incluir la posibilidad de centrarse en las cargas de trabajo críticas

#### 5.3 Expansión de la base de referencia de administración

:book: Según los compromisos empresariales y las decisiones operativas, saca el máximo partido a los procedimientos recomendados que se incluyen para implementar las herramientas necesarias de administración de la nube.

##### Procedimientos recomendados viables

- [Azure Server Management](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/manage/azure-server-management/): guía de incorporación para agregar las herramientas y servicios nativos en la nube necesarios para administrar las operaciones.
- [Supervisión híbrida](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/manage/monitor/): Muchos clientes ya han realizado una inversión sustancial en System Center Operations Manager. Para esos clientes, esta guía sobre la supervisión híbrida puede ayudar a comparar y contrastar las herramientas de notificación nativas de la nube con las herramientas de Operations Manager. Con esta comparación resulta más fácil decidir qué herramientas utilizar para la administración operativa.

#### 5.4 Operaciones avanzadas y principios de diseño

:book: Es posible que las plataformas o cargas de trabajo que necesiten un mayor nivel de compromiso empresarial requieran una revisión más profunda de la arquitectura para cumplir con los compromisos de resistencia y confiabilidad.

![Operaciones avanzadas](/res/images/beyond-the-baseline.png)

## Recursos adicionales

- [Procedimientos recomendados de preparación para Azure](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/ready/azure-best-practices/)

Para aprender más de el consulta los siguientes dos recursos:
- [Aceleración del uso de la nube con Cloud Adoption Framework para Azure](https://docs.microsoft.com/es-mx/learn/modules/build-cloud-governance-strategy-azure/2-accelerate-cloud-adoption-framework)
- [Plataforma de adopción de la nube de Microsoft para Azure](https://docs.microsoft.com/es-es/azure/cloud-adoption-framework/)



# Aspectos Principales Para crear y administrar suscripciones
## Facturación
Se puede crear un informe de facturación por suscripción. Si tenemos varios departamentos y necesitamos realizar un "contracargo" de costes en la nube, una posible solución es organizar las suscripciones por departamento o por proyecto.

## Control de acceso
Una suscripción es un límite de implementación de los recursos de Azure. Cada suscripción está asociada a un inquilino de Azure Active Directory. Cada inquilino proporciona a los administradores la capacidad de configurar un acceso granular a través de roles definidos por medio del control de acceso basado en roles de Azure.

## Límites de suscripción
Las suscripciones también tienen algunas limitaciones de recursos. Por ejemplo, el número máximo de circuitos Azure ExpressRoute de red por cada suscripción es de 10. Estos límites se deben tener en cuenta durante la fase de diseño. Si necesitamos superar estos límites, puede que tengamos que agregar más suscripciones. Si alcanzamos un límite máximo estricto, no hay flexibilidad para aumentarlo.

# ¿Cómo se aplica el control de acceso basado en roles a los recursos?
El control de acceso basado en roles se aplica a un ámbito, que es un recurso o un conjunto de recursos en los que este acceso se permite.
![image](https://user-images.githubusercontent.com/86896526/126711432-66b83a2e-5f48-44f1-810a-2197491979a3.png)
En el diagrama, los observadores, los usuarios que administran recursos, los administradores y los procesos automatizados denotan los tipos de usuarios o cuentas que se suelen asignar a cada uno de los distintos roles.
* Cuando asignamos el rol Propietario a un usuario en el ámbito del grupo de administración, dicho usuario podrá administrar todo el contenido de todas las suscripciones dentro de ese grupo de administración.
* Cuando asignamos el rol Lector a un grupo en el ámbito de suscripción, los miembros de dicho grupo podrán ver todos los grupos de recursos y recursos dentro de esa suscripción.
* Cuando asignamos el rol Colaborador a una aplicación en el ámbito del grupo de recursos, dicha aplicación podrá administrar los recursos de cualquier tipo dentro de ese grupo de recursos específico, pero no los otros grupos de recursos dentro de esa suscripción.

# Control de acceso basados en roles de azure (RBAC de Azure)
## Usaremos RBAC de Azure cuando necesitemos:

* Permitir que un usuario administre las VM en una suscripción y que otro usuario administre las redes virtuales.
* Permitir a un grupo de administradores de base de datos que administren bases de datos SQL de una suscripción
* Permitir que un usuario administre todos los recursos de un grupo de recursos, como las máquinas virtuales, los sitios web y las subredes
* Permitir que una aplicación acceda a todos los recursos de un grupo de recursos.}

### ¿Cómo se aplica RBAC de Azure?
RBAC de Azure se aplica a cualquier acción que se inicie en un recurso de Azure que pasa por Azure Resource Manager. Resource Manager es un servicio de administración que proporciona una forma de organizar y proteger nuestros recursos en la nube.
RBAC emplea un modelo de permisos, es decir, cuando se nos asigna un rol, RBAC nos permite realizar determinadas acciones, como leer, escribir o eliminar. Si una asignación de roles nos concede permisos de lectura a un grupo de recursos y otra asignación de roles nos concede permisos de escritura al mismo grupo de recursos, tendremos permisos tanto de lectura como de escritura en ese grupo de recursos.

### ¿A quién se aplica RBAC de Azure?
RBAC de Azure se puede aplicar a una persona individual o a un grupo. También se puede aplicar a otros tipos de identidad especiales, como entidades de servicio e identidades administradas. Las aplicaciones y los servicios usan estos tipos de identidad para automatizar el acceso a los recursos de Azure.
Los permisos de acceso se administran en el panel Control de acceso (IAM) de Azure Portal.

* Administradores de TI
Este equipo tiene la propiedad definitiva de los recursos tecnológicos, tanto locales como en la nube. El equipo requiere un control completo de todos los recursos.

* Copia de seguridad y recuperación ante desastres
Este equipo es responsable de administrar el estado de las copias de seguridad periódicas y de invocar cualquier recuperación de datos o del sistema.

* Coste y facturación
Los miembros de este equipo realizan un seguimiento e informan sobre los gastos relacionados con la tecnología. También administran los presupuestos internos de la organización.

* Operaciones de seguridad
Este equipo supervisa los incidentes de seguridad relacionados con la tecnología y responde a estos. El equipo requiere acceso continuo a los archivos de registro y a las alertas de seguridad.


# Bloqueos de recursos
Los bloqueos de recursos impiden que se eliminen o modifiquen recursos por error.


Los bloqueos de recursos se pueden administrar en Azure Portal, PowerShell, la CLI de Azure o con una plantilla de Azure Resource Manager.
Para ver, agregar o eliminar bloqueos en Azure Portal, vaya a la sección Configuración del panel Configuración de cualquier recurso en Azure Portal.

### ¿Qué niveles de bloqueo hay disponibles?

* CanNotDelete significa que las personas autorizadas pueden seguir leyendo y modificando un recurso, pero no eliminarlo sin quitar primero el bloqueo.
* ReadOnly significa que las personas autorizadas pueden leer un recurso, pero no eliminarlo ni cambiarlo. Aplicar este bloqueo es como restringir a todos los usuarios autorizados a los permisos concedidos por el rol Lector en RBAC de Azure.

### ¿Cómo se elimina o cambia un recurso bloqueado
Para modificar un recurso bloqueado, primero hay que quitar el bloqueo. Tras quitarlo, podemos aplicar cualquier acción que podamos realizar de acuerdo a nuestros permisos. Este paso adicional nos permite llevar a cabo la acción, e impide que cualquier administrador pueda hacer algo de manera accidental.
Los bloqueos de recursos se aplican con independencia de los permisos RBAC. Es decir, aun siendo el propietario del recurso, tendremos que quitar el bloqueo antes de poder realizar la actividad bloqueada.

# Azure Policy para controlar y auditar recursos

Azure Policy es un servicio de Azure que permite crear, asignar y administrar directivas que controlan o auditan recursos. Dichas directivas aplican distintas reglas y efectos a las configuraciones de los recursos con el propósito de que estas configuraciones sigan cumpliendo con los estándares corporativos.

## ¿Cómo se definen directivas en Azure Policy?
Azure Policy permite definir tanto directivas individuales como grupos de directivas relacionadas (lo que se conoce como iniciativas). Azure Policy evalúa los recursos y resalta los que no cumplen las directivas que hemos creado. Azure Policy también puede impedir que se creen recursos no conformes.

Azure Policy incluye numerosas directivas integradas y definiciones de iniciativas que puede usar, en categorías como Almacenamiento, Redes, Proceso, Centro de seguridad y Supervisión.

## Azure Policy en acción
La implementación de una directiva en Azure Policy conlleva estos tres pasos:

### Crear una definición de directiva
Una definición de directiva expresa qué se debe evaluar y qué acción realizar. Por ejemplo, podemos impedir que se implementen máquinas virtuales en determinadas regiones de Azure.
Cada definición de directiva tiene condiciones que regulan su aplicación. Además, esta definición tiene un efecto complementario que se produce cuando se cumplen las condiciones.

Estos son algunos ejemplos de definiciones de directiva:
* SKU de máquina virtual permitidas.
* Ubicaciones permitidas
* MFA debe estar habilitada en las cuentas con permisos de escritura en la suscripción
* CORS no debe permitir que todos los recursos accedan a las aplicaciones web
* Se deben instalar actualizaciones del sistema en las máquinas


### Asignar la definición a los recursos
Una asignación de directiva es una definición de directiva que se aplica dentro de un ámbito específico. Este ámbito puede ser un grupo de administración (esto es, una colección de varias suscripciones), una sola suscripción o un grupo de recursos.
Todos los recursos secundarios dentro de ese ámbito heredarán las asignaciones de directivas. Si una directiva se aplica a un grupo de recursos, se aplicará también a todos los recursos dentro de ese grupo. Podemos excluir un subámbito de la asignación de directiva si hay recursos secundarios específicos que deban quedar fuera de la asignación de la directiva.


### Revisar los resultados de evaluación
Cuando una condición se evalúa con los recursos existentes, cada recurso se marca como conforme o no conforme. Esto nos permitirá revisar los resultados de directiva que no sean conformes y tomar las medidas oportunas.
La evaluación de la directiva se produce aproximadamente una vez cada hora. Si realizamos cambios en la definición de la directiva y creamos una asignación de directiva, dicha directiva se evaluará con los recursos en una hora

## ¿Qué son las iniciativas Azure Policy?
Una iniciativa de Azure Policy es una forma de agrupar las directivas relacionadas en un mismo conjunto. La definición de iniciativa contiene todas las definiciones de directiva para facilitar el seguimiento del estado de cumplimiento de cara a un objetivo mayor.

## ¿Cómo se asigna una iniciativa?
Al igual que una asignación de directiva, una asignación de iniciativa es una definición de iniciativa que se asigna a un ámbito específico de un grupo de administración, una suscripción o un grupo de recursos.

# Gobernanza de varias suscripciones con Azure Blueprints
puede definir un conjunto repetible de herramientas de gobernanza y recursos de Azure estándar que la organización necesita. De este modo, los equipos de desarrollo pueden crear e implementar rápidamente nuevos entornos sabiendo que se crean de acuerdo con los estándares organizativos con un conjunto de componentes integrados que aceleran las fases de desarrollo e implementación.
Azure Blueprints organiza la implementación de varias plantillas de recursos y de otros artefactos, como son los siguientes:

* Asignaciones de roles
* Asignaciones de directivas
* Plantillas de Azure Resource Manager
* Grupos de recursos

##Cuando formamos un equipo de centro de excelencia en la nube o un equipo de administradores de nube, dicho equipo puede usar Azure Blueprints para escalar sus prácticas de gobernanza en toda la organización.

Para implementar un proyecto en Azure Blueprints hay que realizar estos tres pasos:

Crear una instancia de Azure Blueprints
Asignar ese plano técnico
Llevar un seguimiento de las asignaciones del plano técnico
Con Azure Blueprints, la relación entre la definición del plano técnico (lo que debe ser implementado) y su asignación (lo que se ha implementado) permanece. En otras palabras, Azure crea un registro que asocia un recurso con el plano técnico que lo define, y gracias a esta conexión podemos realizar el seguimiento y la auditoría de nuestras implementaciones.

# Cada componente de la definición de un plano técnico se denomina artefacto.


# Extra
La gobernanza en la nube requiere un buen análisis y recopilar una serie de requisitos. Por suerte, Cloud Adoption Framework para Azure nos puede ayudar a definir e implementar la estrategia de gobernanza. Hay varios servicios y características de Azure que respaldan estos esfuerzos:

- El control de acceso basado en roles de Azure (RBAC de Azure) permite crear roles que definen permisos de acceso.
- Los bloqueos de recursos impiden que se eliminen o modifiquen recursos por error.
- Las etiquetas de recursos proporcionan información extra, o metadatos, sobre los recursos.
- Azure Policy es un servicio de Azure que permite crear, asignar y administrar directivas que controlan o auditan los recursos.
- Azure Blueprints permite definir un conjunto repetible de herramientas de gobernanza y recursos de Azure estándar que la organización necesita.
