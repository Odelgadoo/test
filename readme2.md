# Estructura de Carpetas - Pais

## Descripción
Este proyecto contiene una estructura de carpetas organizada para almacenar scripts relacionados con la operación ETL del país.
El contenedor principal corresponde al país en formato ISO.

## Carpetas Principales

- *0.Admin*: Contiene scripts y configuraciones relacionadas con la administración del sistema.
  - 0.Functions: Scripts que contengan funciones para uso compartido entre procesos ETL.
  - 1.Config: Archivos para manejo de configuraciones, utilizar archivos de configuración (por ejemplo, YAML o JSON) para gestionar parámetros de conexión, rutas de archivos, y otros ajustes relevantes.
  - 2.Logs: Scripts que generen un sistema de registro robusto para capturar eventos, errores y mensajes informativos durante la ejecución del ETL.
  - 3.Error: Scripts que generen un sistema de manejo de excepciones y notificación de errores para garantizar la integridad y confiabilidad del proceso ETL.

- *1.Extract*: Contiene scripts que hace la lectura del archivo de datos del país, desde su fuente original.

- *2.Quality*: Contiene scripts para el análisis descriptivo de la calidad del dato del archivo procesado por 1.Extract, analizando sus dimensiones de calidad y genera archivo DOCX con dicha información. 


- *3.Cleaning*: Contiene scripts para el proceso de limpieza del archivo procesado por 1.Extract consiste en: remover. Duplicados (basado en criterios), conversión de datos a formato numérico, conversión de datos a formato fecha, genera informe de valores atípicos.

- *4.Transform*: Contiene scripts para el proceso de transformación de datos basado en la Matriz de Transformación de datos correspondiente al país. Almacenada en el directorio.

- *5.Load*: Carga de datos en sistemas o bases de datos.

- *6.Orchestrator*: Scripts para orquestar y coordinar los procesos.

- *7.Analysis*: Análisis de datos y scripts para generar informes.

- *99.Misc*: Carpeta miscelánea para archivos diversos.

## Archivos

- *99.Misc/text.txt*: Archivo de texto de ejemplo.

## Uso
Cada carpeta tiene su propósito específico y puede contener subdirectorios para una organización más detallada. Consulta cada carpeta y su descripción para obtener más información sobre su contenido.

---

¡Gracias por visitar nuestro repositorio!
