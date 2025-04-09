# Amazon Books ETL Pipeline

Este proyecto consiste en la creación de una **pipeline ETL** (Extract, Transform, Load) utilizando **Apache Airflow**, cuyo objetivo es extraer datos de libros sobre ingeniería de datos desde Amazon, transformarlos y cargarlos en una base de datos **PostgreSQL**. La pipeline se ejecuta de manera programada para obtener datos actualizados sobre libros de ingeniería de datos.

## Tecnologías Utilizadas

- **Apache Airflow**: Orquestador de flujos de trabajo para crear y administrar la pipeline.
- **PostgreSQL**: Base de datos para almacenar los datos extraídos de Amazon.
- **Docker**: Contenedor para ejecutar la base de datos PostgreSQL y PGAdmin.
- **PGAdmin**: Herramienta de administración para interactuar con la base de datos PostgreSQL.

## Descripción del Proyecto

Este proyecto crea un pipeline ETL que realiza las siguientes tareas:

1. **Extracción (Extract)**: Obtiene datos de libros sobre ingeniería de datos desde Amazon utilizando scraping o APIs (dependiendo de la implementación).
2. **Transformación (Transform)**: Limpia y transforma los datos extraídos, asegurando que estén en un formato adecuado para ser almacenados en la base de datos.
3. **Carga (Load)**: Carga los datos transformados en una base de datos PostgreSQL.

### Objetivos

- Construir una pipeline ETL funcional para la extracción, transformación y carga de datos.
- Almacenar la información de los libros en una base de datos PostgreSQL.
- Visualizar y consultar los datos mediante PGAdmin.

## Instalación

### 1. **Instalar Apache Airflow**

Para instalar Apache Airflow, puedes seguir los siguientes pasos:

```bash
pip install apache-airflow
```

### 2. **Instalar PostgreSQL y PGAdmin usando Docker**

Este proyecto usa Docker para ejecutar PostgreSQL y PGAdmin. Puedes usar los siguientes comandos para levantar los contenedores:

```bash
docker-compose up -d
```

Este comando ejecutará los contenedores de PostgreSQL y PGAdmin.

### 3. **Configuración de PostgreSQL en Airflow**

Dentro de Airflow, configura la conexión a la base de datos PostgreSQL utilizando las credenciales de la base de datos que levantaste en Docker. Esto se puede hacer a través de la interfaz web de Airflow.

## Arquitectura del Pipeline

A continuación, se muestra la arquitectura del pipeline utilizado en este proyecto:

![Arquitectura del Pipeline](https://github.com/Danirive30/Amazon_Books-ETL/blob/main/Pipeline_AB.png)
