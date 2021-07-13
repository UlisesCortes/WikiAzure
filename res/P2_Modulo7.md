# Parte 2 Modulo 7
## Exploración de los servicios de análisis y bases de datos de Azure

## Azure Cosmos BD
Azure Cosmos DB es un servicio de base de datos de varios modelos distribuido globalmente. Puede escalar de forma elástica e independiente el rendimiento y el almacenamiento en cualquier número de regiones de Azure de todo el mundo. Puede aprovechar un acceso rápido y en milisegundos de un solo dígito a los datos mediante cualquiera de las diversas API populares. Azure Cosmos DB proporciona de forma exclusiva contratos de nivel de servicio completos para garantizar el rendimiento, la latencia, la disponibilidad y la coherencia.

Azure Cosmos DB es compatible con los datos sin esquema, lo que le permite compilar aplicaciones "Always On" con una gran capacidad de respuesta para admitir datos en continuo cambio. Puede usar esta característica para almacenar datos actualizados y mantenidos por usuarios de todo el mundo.
Azure Cosmos DB es flexible. En el nivel más bajo, Azure Cosmos DB almacena los datos en formato de secuencia de registro de átomos (ARS). Después, los datos se abstraen y se proyectan como una API, que se especifica al crear la base de datos. Entre las opciones se incluyen SQL, MongoDB, Cassandra, Tables y Gremlin. Este nivel de flexibilidad implica que, al migrar las bases de datos de la empresa a Azure Cosmos DB, los desarrolladores pueden seguir con la API con la que se encuentren más cómodos.

## Azure SQL Database
Azure SQL Database es una base de datos relacional basada en la última versión estable del motor de base de datos de Microsoft SQL Server. SQL Database es una base de datos de alto rendimiento, confiable, totalmente administrada y segura. Puede usarla para compilar aplicaciones y sitios web controlados por datos en el lenguaje de programación que prefiera sin necesidad de administrar infraestructura.

### Características
Azure SQL Database es un motor de base de datos de plataforma como servicio (PaaS). Controla la mayoría de las funciones de administración de bases de datos, como las actualizaciones, las aplicaciones de revisiones, las copias de seguridad y la supervisión, sin intervención del usuario. SQL Database proporciona disponibilidad del 99,99 %. Las capacidades de PaaS que están integradas en SQL Database permiten centrarse en las actividades de administración y optimización de bases de datos específicas del dominio que son críticas para el negocio. SQL Database es un servicio totalmente administrado que ofrece alta disponibilidad, copias de seguridad y otras operaciones de mantenimiento comunes. Microsoft controla todas las actualizaciones del código del sistema operativo y SQL. No hace falta administrar la infraestructura subyacente.

Puede crear una capa de almacenamiento de datos de gran rendimiento y disponibilidad para las aplicaciones y las soluciones de Azure. SQL Database puede ser la opción adecuada para una variedad de aplicaciones modernas en la nube, porque le permite procesar tanto datos relacionales como estructuras no relacionales, por ejemplo, grafos, JSON, elementos espaciales y XML.

Puede usar características avanzadas de procesamiento de consultas, como las tecnologías en memoria de alto rendimiento y el procesamiento de consultas inteligente. De hecho, las funcionalidades más recientes de SQL Server se publican primero en SQL Database y, después, en el propio SQL Server. Las funcionalidades de SQL Server más recientes se obtienen sin costo alguno mediante actualizaciones o mejoras, y se han probado en millones de bases de datos.

### Migración
En la actualidad, Tailwind Traders usa varios servidores locales que ejecutan SQL Server, que proporcionan almacenamiento de datos para el sitio web de acceso público (por ejemplo, datos de clientes, historial de pedidos y catálogos de productos). Además, los servidores locales que ejecutan SQL Server también proporcionan almacenamiento de datos para el sitio web del portal de aprendizaje solo para uso interno. Tailwind Traders usa el sitio web para los materiales de aprendizaje de los nuevos empleados (como los materiales de estudio, los detalles de certificación y los certificados de aprendizaje). En la ilustración siguiente se muestran los tipos de datos que su empresa puede almacenar en el sitio web del portal de aprendizaje de Azure SQL Database.


## Azure Database for MySQL
Azure Database for MySQL es un servicio de bases de datos relacionales en la nube, y se basa en el motor de base de datos de MySQL Community Edition, versiones 5.6, 5.7 y 8.0. Con él, tiene un contrato de nivel de servicio de disponibilidad del 99,99 % de Azure, con la tecnología de una red global de centros de recursos administrados por Microsoft. Esto ayuda a mantener la aplicación ejecutándose de forma ininterrumpida. Con cada servidor de Azure Database for MySQL, se saca provecho de las ventajas de la seguridad integrada, la tolerancia a errores y la protección de datos, algo que de lo contrario tendría que adquirir o diseñar, compilar y administrar. Con Azure Database for MySQL puede usar la restauración a un momento dado para recuperar un servidor a un estado anterior, con un plazo máximo de 35 días.

Azure Database for MySQL ofrece lo siguiente:

* Alta disponibilidad integrada sin coste adicional.
* Rendimiento predecible y precios de pago por uso inclusivos.
* Escalado según sea necesario, en cuestión de segundos.
* Capacidad de protección de información confidencial en reposo y en movimiento.
* Copias de seguridad automáticas.
* Seguridad y cumplimiento de nivel empresarial.


## Azure Database for PostgreSQL
Azure Database for PostgreSQL es un servicio de base de datos relacional en la nube. El software de servidor se basa en la versión de la comunidad del motor de base de datos de PostgreSQL de código abierto. Su familiaridad con las herramientas y la experiencia con PostgreSQL son aplicables cuando se use Azure Database for PostgreSQL.

Además, Azure Database for PostgreSQL ofrece las siguientes ventajas:

* Alta disponibilidad integrada en comparación con los recursos locales. No hay ninguna configuración, replicación o costo adicionales que sean necesarios para asegurarse de que las aplicaciones están siempre disponibles.
* Precios sencillos y flexibles. Tiene un rendimiento predecible en función de un plan de tarifa seleccionado que incluye copias de seguridad automáticas, aplicación de revisiones de software, supervisión y seguridad.
* Escalado o reducción vertical según sea necesario, en cuestión de segundos. Puede escalar procesos o almacenamiento por separado según sea necesario para asegurarse de que adapta su servicio para que coincida con el uso.
* Copias de seguridad automáticas ajustables y restauración a un momento dado durante un máximo de 35 días.
* Seguridad y cumplimiento de nivel empresarial para proteger la información confidencial en reposo y en movimiento. Esta seguridad abarca el cifrado de datos en el disco y el cifrado SSL entre la comunicación entre cliente y servidor.


### Servidor único
Todas estas funcionalidades apenas requieren tareas de administración y todas se proporcionan sin costo adicional. Se puede centrar en el desarrollo rápido de aplicaciones y en reducir el plazo de comercialización, en lugar de tener que administrar las máquinas virtuales y la infraestructura. Puede seguir desarrollando la aplicación con las herramientas de código abierto y en la plataforma de que prefiera sin necesidad de adquirir nuevos conocimientos.

### Hiperescala (Citus)

La opción de Hiperescala (Citus) escala horizontalmente las consultas entre varias máquinas mediante el particionamiento. Su motor de consultas paraleliza las consultas SQL entrantes en estos servidores para agilizar las respuestas en conjuntos de datos grandes. Proporciona servicios a las aplicaciones que requieren mayor escala y mejor rendimiento, por lo general las cargas de trabajo que se aproximan a los 100 GB de datos (o que ya los superan).

## Azure SQL Managed Instance
Azure SQL Managed Instance es un servicio de datos en la nube escalable que proporciona la mayor compatibilidad con el motor de base de datos de SQL Server con todas las ventajas de una plataforma como servicio totalmente administrada. En función de su escenario, Azure SQL Managed Instance podría ofrecer más opciones para sus necesidades de base de datos.

### Características
Es un motor de base de datos de plataforma como servicio (PaaS), lo que significa que su empresa podrá aprovechar las mejores características de mover los datos a la nube en un entorno totalmente administrado. Por ejemplo, su empresa ya no necesitará comprar y administrar hardware caro, y no tendrá que mantener la sobrecarga adicional derivada de administrar la infraestructura local. Por otro lado, su empresa se beneficiará de las características de aprovisionamiento rápido y escalado de servicio de Azure, junto con la aplicación automatizada de revisiones y las actualizaciones de versiones. Además, podrá estar seguro de que los datos siempre estarán allí cuando los necesite a través de características de alta disponibilidad integradas y un acuerdo de nivel de servicio (SLA) del 99,99 % de tiempo de actividad. También podrá proteger los datos con copias de seguridad automatizadas y un período de retención de copias de seguridad configurable.

Azure SQL Database y Azure SQL Managed Instance ofrecen muchas características iguales, pero Azure SQL Managed Instance proporciona varias opciones que puede que no estén disponibles en Azure SQL Database. Por ejemplo, Tailwind Traders usa actualmente varios servidores locales que ejecutan SQL Server y les gustaría migrar sus bases de datos existentes a una base de datos SQL que se ejecute en la nube. Sin embargo, algunas de sus bases de datos usan caracteres cirílicos para la intercalación. En este escenario, Tailwind Traders debe migrar sus bases de datos a una instancia de Azure SQL Managed Instance, ya que Azure SQL Database solo usa la intercalación del servidor SQL_Latin1_General_CP1_CI_AS predeterminada.

### Migración
Azure SQL Managed Instance facilita la migración de los datos locales en SQL Server a la nube con Azure Database Migration Service (DMS) o copias de seguridad y restauración nativas. Una vez que haya descubierto todas las características que usa la empresa, deberá evaluar qué instancias locales de SQL Server puede migrar a Azure SQL Managed Instance para ver si tiene algún problema de bloqueo. Una vez resueltas las incidencias, puede migrar los datos y, después, realizar la transferencia desde el servidor SQL Server local a la instancia de Azure SQL Managed Instance cambiando la cadena de conexión en las aplicaciones.

## Exploración de análisis y microdatos
### Azure Synapse Analytics

Azure Synapse Analytics (anteriormente Azure SQL Data Warehouse) es un servicio de análisis ilimitado que reúne el almacenamiento de datos empresariales y el análisis de macrodatos. Puede consultar los datos como prefiera mediante recursos sin servidor o aprovisionados a escala. Tiene una experiencia unificada para ingerir, preparar, administrar y servir datos para las necesidades inmediatas de inteligencia empresarial y aprendizaje automático.

### Azure HDInsight

Azure HDInsight es un servicio de análisis de código abierto totalmente administrado para empresas. Es un servicio en la nube que hace que sea más fácil, rápido y rentable procesar grandes cantidades de datos. Puede ejecutar marcos de código abierto populares y crear tipos de clúster, como Apache Spark, Apache Hadoop, Apache Kafka, Apache HBase, Apache Storm y Machine Learning Services. HDInsight también admite una amplia gama de escenarios, como la extracción, la transformación y la carga de datos (ETL), el almacenamiento de datos, el aprendizaje automático e IoT.

### Azure Databricks

Azure Databricks le ayuda a descubrir información de todos los datos y a crear soluciones de inteligencia artificial. Puede configurar el entorno de Apache Spark en minutos y, después, escalar automáticamente y colaborar en proyectos compartidos en un área de trabajo interactiva. Azure Databricks admite Python, Scala, R, Java y SQL, así como marcos y bibliotecas de ciencia de datos, como TensorFlow, PyTorch y Scikit-learn.


### Análisis con Azure Data Lake

Azure Data Lake Analytics es un servicio de trabajos de análisis a petición que simplifica los macrodatos. En lugar de implementar, configurar y ajustar el hardware, escribirá consultas para transformar los datos y extraer ideas valiosas. El servicio de análisis puede administrar trabajos de cualquier escala al instante, simplemente estableciendo el ajuste adecuado. Solo paga por su trabajo cuando se está ejecutando, lo que hace que sea más rentable.
