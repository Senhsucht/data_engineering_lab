# ☁️ Cloud Data Engineering Lab

Este directorio contiene ejercicios y proyectos prácticos de **Data Engineering en la nube**, desarrollados como parte de mi portafolio profesional.  
El objetivo es demostrar habilidades en integración de datos, orquestación de flujos ETL/ELT, almacenamiento en diferentes formatos y conexión con herramientas de análisis.

---

## 📂 Estructura

cloud/
├── azure/ # Proyectos en Azure Data Factory, Storage, Power BI
├── aws/ # (futuro) Ejercicios en AWS Glue, S3, Redshift
└── gcp/ # (futuro) Ejercicios en BigQuery, Dataflow, GCS

---

## 🚀 Proyectos implementados

### 🔹 [Azure - Flights Delay Pipeline](./azure)
Pipeline en **Azure Data Factory (ADF)** que:
- Unifica datos de vuelos del primer trimestre 2020.
- Filtra registros sin valores nulos en retrasos de despegue y aterrizaje.
- Calcula métricas de % de retrasos por aerolínea, origen y destino.
- Guarda el resultado en formato **Parquet particionado** en Blob Storage.

[👉 Ver proyecto completo](./azure)

---

## 📌 Próximos pasos
- Extender la solución con dashboards en **Power BI**.  
- Crear versiones en **AWS** y **GCP** para comparar servicios equivalentes.  
- Explorar **automatización CI/CD** con GitHub Actions y despliegue en la nube.
