# 🐍 PySpark Exercises

Esta carpeta contiene ejercicios prácticos de **PySpark**, diseñados para reforzar el uso de Spark en procesamiento de datos distribuidos.  
Los ejercicios están enfocados en operaciones comunes de **Data Engineering**, como limpieza, transformaciones, joins y agregaciones.

---

## 📂 Estructura
Se generar una carpeta por proyecto cada uno tendra:

├── data/                       # datasets de entrada
├── notebooks/                  # versión en notebook
├── src/                        # código PySpark modularizado
├── output/                     # aquí se guardan los Parquet generados
└── README.md                   # explicación del proyecto


---

## 🎯 Objetivos de la carpeta

- Familiarizarse con la **API de PySpark**.  
- Practicar la creación de **pipelines de transformación de datos**.  
- Reforzar conceptos clave:
  - Lectura y escritura de datos (CSV, Parquet, Delta).
  - Transformaciones (`select`, `withColumn`, `filter`, `drop`).
  - Joins (`inner`, `left`, `right`, `outer`).
  - Funciones de agregación y **Window functions**.
  - Manejo de errores y buenas prácticas en scripts PySpark.

---

## ⚡ Ejecución

1. Inicia sesión en tu entorno PySpark (local o Databricks).  
   Ejemplo en local:

```bash
   pyspark
```

o usando spark-submit:

```bash
spark-submit ejercicio_01_basico.py
```

2. Revisa la salida en consola o los archivos generados en output/.