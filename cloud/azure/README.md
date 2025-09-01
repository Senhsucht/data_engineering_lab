# Azure - Flights Delay Pipeline

Este ejercicio forma parte del portafolio **data_engineering_lab** y tiene como objetivo practicar con **Azure Data Factory (ADF)** para construir un flujo ETL sencillo en la nube.

## 🎯 Objetivo
Unificar datos de vuelos del primer trimestre de 2020, limpiarlos y obtener métricas de retrasos en despegue y aterrizaje, almacenando el resultado en formato **Parquet particionado**.

## 🏗️ Arquitectura
- **Azure Storage Account (Blob Storage)**: Contiene los archivos CSV de vuelos.
- **Azure Data Factory (ADF)**: Orquesta el flujo de datos.
- **Sink**: Almacena los resultados procesados en formato Parquet.

Diagrama simple:

CSV (Blob Storage) --> ADF Pipeline (Transformaciones) --> Parquet particionado (Sink)


## ⚙️ Pipeline en ADF
El Data Flow dentro del pipeline sigue estos pasos:

1. **Source**: lee los CSV desde el Blob Storage.  
2. **Select**: selecciona columnas relevantes (`Carrier`, `Origin`, `Dest`, `DEP_DEL15`, `ARR_DEL15`).  
3. **Filter**: elimina filas con valores nulos en `DEP_DEL15` y `ARR_DEL15`. 
4. **Aggregate**: calcula porcentaje de retrasos por aerolínea, origen y destino.  
5. **Sink**: guarda la salida en formato **Parquet particionado** por aerolínea.

## ✅ Resultado esperado
Un dataset en formato **Parquet particionado** con las siguientes métricas:

- % retrasos en despegue (`DEP_DEL15`)  
- % retrasos en aterrizaje (`ARR_DEL15`)  

## 🚀 Posibles mejoras
- Conectar la salida en Parquet a **Power BI** para crear dashboards de visualización.  
- Incorporar más periodos de datos y automatizar la carga incremental.  
- Integrar **Azure SQL Database** como destino alternativo.