📸 Proyecto Instagram DataPipeline
Pipeline de datos masivos usando Azure Data Factory, Databricks y Azure Blob Storage.

📝 Descripción
Este proyecto demuestra la orquestación de un flujo ETL a gran escala, procesando más de 1.5 millones de registros del dataset Instagram Lifestyle.
El objetivo es transformar datos crudos de comportamiento de usuarios desde la zona Raw hasta una zona Procesada, lista para análisis.

🛠️ Arquitectura Tecnológica
Azure Data Factory (ADF) → orquestación y movimiento de datos.

Azure Databricks (PySpark) → procesamiento distribuido y capa Silver.

Azure Blob Storage → almacenamiento estructurado en capas (Raw/Processed).

GitHub → control de versiones de la infraestructura de datos.

⚙️ Flujo del Pipeline
Ingesta → datos recibidos en contenedores de Blob Storage.

Procesamiento → Databricks con optimización de memoria para alto volumen.

Orquestación → ADF con:

Datasets parametrizados.

Rutas comodín (*) para múltiples archivos Spark.

SAS Tokens para seguridad y gobernanza.

📊 Resultados Técnicos
Volumen procesado: ~440 MB.

Rendimiento: 73,28 MB/s de transferencia.

Escalabilidad: copias en paralelo con múltiples DIU en Azure.

🛡️ Gobernanza y Seguridad
Políticas de acceso con SAS Tokens.

Principio de mínimo privilegio aplicado en permisos de lectura/escritura.

👤 Autor
Mauricio Vélez Rengifo  
Ingeniero de Datos | Desarrollador Backend

GitHub: Mvelezrengifo

LinkedIn: Mauricio Vélez
