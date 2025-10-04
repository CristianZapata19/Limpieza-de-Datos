Limpieza y Preparación de Datos: Sueño y Estilo de Vida

Este proyecto documenta el riguroso proceso de Limpieza de Datos (Data Wrangling) aplicado al conjunto Sleep_health_and_lifestyle_dataset.csv. El objetivo es transformar los datos crudos en una fuente confiable y estructurada para el análisis.

Resultado del Proceso de Limpieza

Se resolvieron siete (7) problemáticas críticas que comprometían la calidad del dataset. El código completo de estas intervenciones se encuentra en el Jupyter Notebook asociado.

1. Limpieza Estructural
Duplicados Eliminados: Se eliminaron 242 filas duplicadas, garantizando 132 registros únicos.

Nombres Estandarizados: Se aplicó formato snake_case y traducción a todas las columnas (Sleep Duration → duracion_sueno_horas).

Columna Compuesta Separada: La columna Blood Pressure fue dividida en dos variables numéricas: presion_sistolica y presion_diastolica.

2. Coherencia de Valores y Tipos

Valores Nulos Corregidos: Los NaN en trastorno_sueno fueron imputados con la etiqueta ninguno.

Inconsistencia Categórica (IMC): Se unificaron las etiquetas 'Normal Weight' a 'Normal'.

Inconsistencia Categórica (Trastornos): Las etiquetas fueron estandarizadas a minúsculas y traducidas al español (p. ej., Insomnia → insomnio).

Granularidad Numérica Ajustada: La columna duracion_sueno_horas se redondeó a un decimal para mejorar la consistencia analítica.

Conclusión

La aplicación de esta limpieza integral asegura que el conjunto de datos está listo para la fase de Análisis Exploratorio de Datos (EDA) y posterior modelización, sin sesgos causados por duplicados o inconsistencias.

