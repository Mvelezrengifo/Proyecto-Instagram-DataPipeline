# Proyecto-Instagram-DataPipeline
"Pipeline de datos masivos usando Azure Data Factory, Databricks y Azure Blob Storage".

Pipeline de Procesamiento Masivo: Instagram Lifestyle Dataset 🚀
📝 Descripción del Proyecto
Este proyecto demuestra la orquestación de un flujo de datos (ETL) a gran escala, procesando más de 1.5 millones de registros. El objetivo fue transformar datos crudos de comportamiento de usuarios en Instagram desde una zona de aterrizaje (Raw) hasta una zona procesada lista para analítica.

🛠️ Arquitectura Tecnológica
Azure Data Factory (ADF): Orquestación del pipeline y movimiento de datos.

Azure Databricks (PySpark): Procesamiento distribuido y transformación de la capa Silver.

Azure Blob Storage: Almacenamiento estructurado en capas (Raw/Processed).

GitHub Integration: Control de versiones para toda la infraestructura de datos.

⚙️ Flujo del Pipeline
Ingesta: Los datos se reciben en contenedores de Azure Blob Storage.

Procesamiento: Uso de Databricks con optimización de memoria para manejar el volumen masivo de filas.

Orquestación: Creación de un pipeline en ADF utilizando:

Datasets parametrizados.

Wildcard File Paths (*): Para ingesta de múltiples archivos generados por Spark.

SAS Tokens: Implementación de seguridad y gobernanza en el acceso a datos.

📊 Resultados Técnicos
Volumen: ~440 MB de datos procesados.

Rendimiento: Tasa de transferencia de 73.28 MB/s.

Escalabilidad: Implementación de copias en paralelo utilizando múltiples DIUs en Azure.

🛡️ Gobernanza y Seguridad
Se aplicaron políticas de acceso mediante firmas de acceso compartido (SAS) para limitar los permisos de escritura/lectura entre servicios, siguiendo el principio de "mínimo privilegio".
