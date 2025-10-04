Limpieza de Datos: Salud y Estilo de Vida del Sueño

Visión General del Proyecto

Este proyecto documenta el proceso completo de Limpieza y Estandarización de Datos (Data Wrangling) aplicado al dataset Sleep_health_and_lifestyle_dataset.csv.

El objetivo principal es transformar un conjunto de datos crudo con inconsistencias, duplicados y valores atípicos en una fuente de información limpia, coherente y lista para el Análisis Exploratorio de Datos (EDA) y la modelización posterior.

Herramientas Utilizadas
Lenguaje: Python

Librerías: Pandas

Entorno: Jupyter Notebook (o entorno similar)

📋 Problemáticas de Limpieza Resueltas
Se identificaron y corrigieron siete (7) problemáticas clave en el dataset que comprometían la calidad del análisis.

#	Problemática	Intervención
1	Duplicados Exactos	Eliminación de 242 filas duplicadas para asegurar la unicidad de los registros.
2	Nombres Inconsistentes	Estandarización de nombres de columnas a snake_case y traducción al español.
3	Columna Compuesta	División de Blood Pressure en dos columnas numéricas: presion_sistolica y presion_diastolica.
4	Datos Faltantes	Imputación de valores NaN en trastorno_sueno con la categoría ninguno.
5	Inconsistencia Categórica (IMC)	Unificación de las etiquetas 'Normal Weight' a 'Normal' en categoria_imc.
6	Inconsistencia Categórica (Trastornos)	Estandarización de mayúsculas/minúsculas y traducción de etiquetas en trastorno_sueno.
7	Granularidad Numérica	Redondeo de duracion_sueno_horas a un decimal para mejorar la consistencia analítica.
Ejecutar las celdas en orden. Asegúrese de que el archivo .csv esté en el mismo directorio raíz. El notebook documenta y verifica el estado de los datos en cada paso.

Hecho por [Tu Nombre] para [Nombre de la Asignatura/Curso]
