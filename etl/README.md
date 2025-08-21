# 🛠️ ETL Labs

Este directorio contiene ejercicios y proyectos de **ETL (Extract, Transform, Load)**, desarrollados como parte de mi práctica en Data Engineering.  

## 📂 Estructura del proyecto

ETL/
│── datasets/ # Archivos de datos de entrada (CSV, JSON, etc.)
│── notebooks/ # Notebooks de Jupyter o Google Colab con análisis y pruebas
│── outputs/ # Resultados generados después del proceso ETL
│── scripts/ # Scripts en Python/SQL para las transformaciones
│── README.md # Documentación del proyecto

---

## 🚀 Objetivo
  
Practicar los conceptos clave de un flujo **ETL**:

1. **Extract** → Cargar datos desde diferentes fuentes (archivos CSV, JSON, APIs, etc.).  
2. **Transform** → Limpiar, normalizar y aplicar reglas de negocio.  
3. **Load** → Exportar los datos listos hacia un archivo limpio, base de datos o data warehouse.  

## 📋 Ejercicios

1. [**Ejercicio 1**:Limpieza de CSV](notebooks/etl_ejercicio1.ipynb)
2. [**Ejercicio 2**:Agregación de Datos](notebooks/etl_ejercicio2.ipynb)
3. [**Ejercicio 3**:Unión de Tablas y Agregación](notebooks/etl_ejercicio3.ipynb)

---


## ⚙️ Requisitos

- Python 3.10+  
- Librerías principales:  

 ```bash
  pip install pandas numpy sqlalchemy
  ```

  (Opcional si usas notebooks: `jupyter` o `jupyterlab`)

## ▶️ Cómo ejecutar

1. Clonar el repositorio:
    `git clone <url_del_repositorio> cd ETL`
2. Ejecutar un script de ejemplo:
    `python scripts/etl_ejercicio1.py`
3. Revisar los resultados en la carpeta `outputs/`.
  
---
## 📖 Notas

- Cada ejercicio tiene su propio script o notebook.
- Los datasets son de uso educativo.
- Este proyecto está pensado únicamente para práctica personal.

✍️ Autor: Angel Arturo Castro Cortes