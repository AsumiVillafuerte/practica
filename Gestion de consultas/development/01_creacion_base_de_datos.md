# BASE DE DATOS EN MYSQL

1. [MYSQL](#mysql)
2. [Gestión de base de datos](#gestion-de-base-de-datos)
   * [Crear base de datos](#crear-base-de-datos)
   * [Archivos físicos de la base de datos](#archivos-fisicos-de-la-base-de-datos)
   * [Poner en uso de la base de datos](#poner-en-uso-de-la-base-de-datos)
   * [Inventario de base de datos](#inventario-de-base-de-datos)
   * [Eliminar base de datos](#eliminar-base-de-datos)
3. [Creación de base de datos PRO](#creacion-de-base-de-datos-pro)



## MySQL

1. Es uno de los SGBD más populares en el mundo.
2. MySQL Community Edition (5.x) VS MySQL Enterprise Edition (8.x)
3. Existe una gran comunidad y documentación disponible.
4. Se integra facilmente con lenguajes de programación populares.
5. Se adapta a una gran variedad de aplicaciones simples y complejas.

## GESTION DE BASE DE DATOS
1. Es el contenedor principal de todos los objetos de una base de datos.
2. Objetos: tablas, vistas, cursores, índices, procedimientos almacenados, etc.

### CREAR BASE DE DATOS

1. Sintaxis para crear una base de datos:

````SQL
CREATE DATABASE formulario;
````

### ARCHIVOS FISICOS DE LA BASE DE DATOS

1. Los archivos físicos tienen la extensión: opt, frm e ibd.
2. Sintaxis para visualizar la ubicación de los archivos físicos de la base de datos:

````SQL
SHOW VARIABLES LIKE 'datadir';
````

### PONER EN USO DE LA BASE DE DATOS

1. Sintaxis para poner en uso de la base de datos:

````SQL
USE formulario;
````

### INVENTARIO DE BASE DE DATOS

1. Sintaxis para listar las base de datos:

````SQL
SHOW DATABASES;
````

### ELIMINAR BASE DE DATOS

1. Antes de eliminar una base de datos, esta no debe estar en uso.
2. Para saber que base de datos está en uso utilice: SELECT DATABASE();
3. Poner otra base de datos en uso: USE sakila;
4. Para eliminar una base de datos utilice DROP DATABASE.
5. Sintaxis para eliminar una base de datos:

````SQL
DROP DATABASE formulario ;
````

7. Verificar si se ha eliminado haciendo un listado de base de datos.

````SQL
SHOW DATABASES;
````

8. Tener presente que el eliminado es una operación irreversible.

## CREACION DE BASE DE DATOS PRO

````SQL
CREATE DATABASE IF NOT EXISTS formulario
CHARACTER SET utf8mb4 
COLLATE utf8mb4_spanish_ci;
USE formulario;
````