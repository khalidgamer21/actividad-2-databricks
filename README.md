# Actividad 2: procesamiento de datos en Databricks

Este repositorio contiene el notebook desarrollado por **Marlon Monterrosa,
Yimy Mosquera y Rafael Gonzalez** para practicar la ingesta, almacenamiento y
validación de datos en una infraestructura cloud.

## ¿Qué hicimos?

Trabajamos con el dataset público **Iris** de Kaggle, compuesto por 150
registros de flores de tres especies diferentes.

El proceso realizado fue:

1. Configurar y documentar el entorno Serverless de Databricks.
2. Descargar el dataset desde Kaggle mediante su API.
3. Almacenar el archivo CSV en un Unity Catalog Volume.
4. Leer los datos con PySpark aplicando un esquema explícito.
5. Validar registros nulos, duplicados, tipos de datos y cantidades.
6. Crear la tabla Delta `workspace.actividad_2.iris`.
7. Comparar consultas y agrupaciones realizadas con PySpark y SQL.

## Tecnologías utilizadas

- Databricks Community Edition con cómputo Serverless
- Apache Spark y PySpark
- Spark SQL
- Delta Lake
- Unity Catalog Volumes
- API de Kaggle

## Resultados principales

Las validaciones confirmaron que el dataset contiene **150 registros**, sin
identificadores duplicados ni valores nulos. También se comprobó que existen
tres especies con **50 observaciones cada una**.

PySpark resultó útil para definir el esquema, automatizar controles y crear la
tabla. SQL permitió consultar rápidamente los metadatos, conteos, filtros y
promedios agrupados.

## Archivo de la entrega

El notebook incluye el código, las explicaciones y las salidas obtenidas
durante la ejecución:

- [`Monterrosa_Marlon_Actividad_2.ipynb`](Monterrosa_Marlon_Actividad_2.ipynb)

- link del video: https://drive.google.com/drive/folders/1bjBUKoZ-c8WbA4P-yxwth62fTMHnoC-T?usp=sharing

Las credenciales utilizadas para acceder a Kaggle fueron eliminadas antes de
publicar la entrega.
