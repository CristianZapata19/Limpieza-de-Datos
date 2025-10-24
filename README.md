

# Limpieza y Preparación de Datos: Sueño y Estilo de Vida

## Descripción General del Proyecto

Este proyecto documenta el riguroso proceso de Limpieza de Datos (Data Wrangling) aplicado al conjunto de datos `Sleep_health_and_lifestyle_dataset.csv`. El objetivo principal es transformar los datos crudos en una fuente confiable, coherente y estructurada, preparándola para un análisis de datos preciso.

El código completo que detalla cada una de estas intervenciones se encuentra en el Jupyter Notebook (`.ipynb`) incluido en este repositorio.

---

## Resumen del Proceso de Limpieza

Durante la preparación de los datos, se identificaron y resolvieron **siete (7) problemáticas críticas** que comprometían la calidad e integridad del conjunto de datos.

### 1. Limpieza Estructural

Se corrigieron problemas relacionados con la forma y estructura del DataFrame:

* **Eliminación de Duplicados:** Se identificaron y eliminaron **242 filas duplicadas**, garantizando 132 registros únicos y fiables.
* **Estandarización de Nombres:** Se aplicó formato `snake_case` y se tradujeron todos los nombres de las columnas al español (p. ej., `Sleep Duration` → `duracion_sueno_horas`).
* **Separación de Columnas:** La columna `Blood Pressure` (presión arterial), que era un valor compuesto, se dividió en dos variables numéricas independientes: `presion_sistolica` y `presion_diastolica`.

### 2. Coherencia de Valores y Tipos

Se normalizaron los datos dentro de las columnas para asegurar la consistencia:

* **Imputación de Nulos:** Los valores nulos (`NaN`) en la columna `trastorno_sueno` fueron imputados con la etiqueta categórica 'ninguna', asumiendo que la ausencia de datos implica la ausencia del trastorno.
* **Unificación Categórica (IMC):** Se unificaron las etiquetas inconsistentes para el Índice de Masa Corporal. Por ejemplo, 'Peso Normal' se estandarizó a 'Normal'.
* **Unificación Categórica (Trastornos):** Las etiquetas en la columna de trastornos del sueño se estandarizaron a minúsculas y se tradujeron al español (p. ej., `Insomnia` → `insomnio`).
* **Ajuste de Granularidad:** Los valores en `duracion_sueno_horas` se redondearon a un solo decimal para mejorar la consistencia analítica.

---

## Conclusión

Tras la aplicación de esta limpieza integral, el conjunto de datos se considera robusto y listo para las siguientes fases del análisis, como el **Análisis Exploratorio de Datos (EDA)** y el posterior desarrollo de **modelos de machine learning**. Se han mitigado los sesgos potenciales causados por duplicados, valores nulos e inconsistencias categóricas.
