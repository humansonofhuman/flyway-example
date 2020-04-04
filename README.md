# flyway-example
Ejemplo de como utilizar docker-compose y flyway para montar una base de datos con estructura y datos para desarollo

## Estructura del proyecto
Dentro del proyecto se encuentra una carpeta por cada base de datos de la que se da ejemplo

Dentro de la carpeta hay un docker-compose con las instrucciones para levantar la base de datos y realizar la migración con flyway.

La carpeta database contiene otra carpeta flyway donde están los archivos con los que se construye la estructura de la base de datos
y se inserta la información

```txt      
postgresql
├── docker-compose.yml
└── database
    └── flyway
        ├── V1__create_schema.sql
        └── V1.1__load_initial_data.sql
mysql
├── docker-compose.yml
└── database
    └── flyway
        ├── V1__create_schema.sql
        └── V1.1__load_initial_data.sql
```

## Pre requisitos

- Tener instalado [Docker Desktop](https://www.docker.com/products/docker-desktop)

## Como correr el proyecto

- cd postgrsql
- docker-compose up
