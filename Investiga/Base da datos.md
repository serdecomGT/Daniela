# BASES DE DATOS
---

¿Qué es una base de datos?

Una base de datos es un conjunto organizado de información que se almacena de manera estructurada para poder guardar, consultar, modificar, eliminar y administrar datos de forma rápida y eficiente.

Las bases de datos están presentes en muchas actividades de la vida cotidiana. Por ejemplo, cuando una escuela registra estudiantes y calificaciones, cuando un hospital guarda información de sus pacientes, cuando una tienda controla sus productos o cuando una aplicación almacena información de sus usuarios, normalmente está utilizando una base de datos.

Una base de datos permite manejar grandes cantidades de información sin tener que buscar cada dato manualmente. Para trabajar con ella normalmente se utiliza un Sistema Gestor de Bases de Datos (SGBD o DBMS).

## ¿Para qué sirve una base de datos?

Las bases de datos sirven principalmente para organizar y administrar información. Entre sus funciones se encuentran:

Guardar información de manera organizada.
Buscar datos rápidamente.
Agregar nuevos registros.
Modificar información existente.
Eliminar datos que ya no son necesarios.
Evitar la duplicación innecesaria de información.
Relacionar diferentes tipos de información.
Controlar el acceso de los usuarios.
Mantener la información disponible para diferentes aplicaciones.
Generar informes y estadísticas.

Por ejemplo, una tienda puede utilizar una base de datos para saber cuántos productos tiene disponibles, cuáles se han vendido, cuánto cuestan y quién realizó una compra.

## Elementos de una base de datos

Una base de datos puede estar formada por diferentes elementos dependiendo del tipo de sistema que se utilice.

1. Datos
Son la información que se almacena.

Ejemplo:
Nombre: Daniela
Edad: 17
Curso: 5to Computación

2. Tablas
En las bases de datos relacionales, las tablas sirven para organizar los datos en filas y columnas.

Por ejemplo, una tabla llamada Estudiantes podría tener:
ID	Nombre	Edad	Curso
1	Daniela	17	5to Computación
2	Carlos	18	5to Computación
3	Ana	17	5to Computación
3. Campos

Los campos son las columnas de una tabla y representan las características de los datos.

En el ejemplo anterior:
ID
Nombre
Edad
Curso

son campos.

4. Registros
Un registro es cada fila de una tabla y contiene información relacionada con un elemento.

5. Claves

Las claves sirven para identificar y relacionar información.
La más conocida es la clave primaria (Primary Key), que identifica de forma única cada registro.

Por ejemplo:
ID = 1

puede identificar exclusivamente a una estudiante.

## ¿Qué es una clave primaria?

Una clave primaria es un campo que permite identificar de manera única cada registro dentro de una tabla.

Por ejemplo:
ID	Nombre	Edad
1	Ana	17
2	Luis	18
3	Carlos	17

El campo ID puede funcionar como clave primaria porque no debería repetirse.
Esto ayuda a evitar confusiones cuando existen personas con el mismo nombre.

## ¿Qué es una clave foránea?

Una clave foránea (Foreign Key) es un campo que permite relacionar una tabla con otra.

Por ejemplo, podemos tener:
Tabla Estudiantes

ID	Nombre
1	Ana
2	Carlos

Tabla Cursos

ID_Curso	Curso	ID_Estudiante
101	Computación	1
102	Matemática	2

El campo ID_Estudiante puede relacionarse con el ID de la tabla de estudiantes.

Así se pueden conectar diferentes informaciones.

## ¿Qué es SQL?

SQL significa Structured Query Language, que en español significa Lenguaje de Consulta Estructurado.

Es un lenguaje utilizado principalmente para trabajar con bases de datos relacionales.

Con SQL podemos:

Crear tablas.
Insertar información.
Consultar datos.
Modificar registros.
Eliminar información.
Crear relaciones.
Controlar permisos.

Ejemplo:

SELECT * FROM Estudiantes;
Esta instrucción solicita todos los datos de la tabla Estudiantes.

Otro ejemplo:

INSERT INTO Estudiantes (Nombre, Edad)
VALUES ('Daniela', 17);

Esta instrucción agrega un nuevo estudiante.

## ¿Qué es un Sistema Gestor de Bases de Datos?

Un Sistema Gestor de Bases de Datos (SGBD) es un programa que permite crear, administrar y utilizar bases de datos.

El gestor funciona como intermediario entre el usuario o una aplicación y la información almacenada.

Algunos gestores conocidos son:

MySQL

Es uno de los sistemas de gestión de bases de datos más utilizados y es muy común en aplicaciones web.

PostgreSQL

Es un sistema de código abierto conocido por sus características avanzadas y su capacidad para manejar aplicaciones complejas.

SQL Server

Es desarrollado por Microsoft y se utiliza en muchas empresas y sistemas profesionales.

Oracle Database

Es una solución utilizada principalmente en organizaciones que necesitan administrar grandes cantidades de información.

MongoDB

Es una base de datos NoSQL que almacena información utilizando documentos, en lugar de organizarla exclusivamente mediante tablas.

## ¿Cómo funciona una base de datos?

De manera sencilla, el funcionamiento puede representarse así:

Por ejemplo, cuando una persona inicia sesión en una aplicación:

El usuario introduce su nombre y contraseña.
La aplicación recibe esos datos.
La aplicación realiza una consulta a la base de datos.
El sistema gestor busca la información.
La base de datos devuelve el resultado.
La aplicación muestra al usuario si los datos son correctos.
Operaciones básicas

Las bases de datos permiten realizar cuatro operaciones fundamentales conocidas como CRUD:
Create — Crear

Permite agregar nuevos datos.
Read — Leer

Permite consultar información.
Update — Actualizar

Permite modificar información existente.
Delete — Eliminar
   
Permite borrar información.

## Seguridad en las bases de datos

La seguridad es muy importante porque las bases de datos pueden contener información privada o importante.

Algunas medidas de seguridad son:

Contraseñas.
Usuarios y permisos.
Cifrado.
Copias de seguridad.
Control de acceso.
Auditorías.
Actualizaciones del sistema.
Protección contra accesos no autorizados.

Por ejemplo, no todos los empleados de una empresa deberían tener permiso para modificar información financiera.

## Copias de seguridad

Una copia de seguridad o backup es una copia de los datos que permite recuperarlos si ocurre algún problema.

Puede ser necesaria cuando:

Se daña un equipo.
Se eliminan datos accidentalmente.
Ocurre un fallo del sistema.
Se produce un ataque informático.
Se pierde información.

Por eso, las organizaciones suelen realizar copias de seguridad periódicamente.

## Datos interesantes
Una base de datos puede almacenar millones o incluso miles de millones de registros.
Muchas aplicaciones que utilizamos diariamente dependen de bases de datos aunque el usuario no las vea.
Las bases de datos pueden trabajar simultáneamente con información de muchos usuarios.
SQL es uno de los lenguajes más importantes para trabajar con bases de datos relacionales.
Una base de datos puede estar almacenada en un servidor local o en servicios de computación en la nube.
Las bases de datos son fundamentales para el funcionamiento de sitios web, aplicaciones móviles y sistemas empresariales.
Una mala organización de los datos puede provocar errores, información duplicada y problemas en un sistema.


## Importancia de las bases de datos

Las bases de datos son fundamentales en la informática porque permiten convertir grandes cantidades de información en datos organizados y fáciles de administrar. Sin ellas, sería mucho más complicado desarrollar sistemas como bancos en línea, tiendas virtuales, plataformas educativas, aplicaciones móviles, hospitales y redes sociales.

## En conclusión
una base de datos no es simplemente un lugar donde se guarda información, sino una herramienta que permite organizar, relacionar, consultar, proteger y administrar datos de manera eficiente. Por esta razón, aprender sobre bases de datos es muy importante para cualquier persona que estudie informática, programación o desarrollo de sistemas.
