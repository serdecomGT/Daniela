# Plan de desarrollo de la aplicación
El proyecto consiste en desarrollar una aplicación móvil multiplataforma utilizando C#, Blazor, .NET MAUI y SQLite, con el propósito de llevar un control organizado de la asistencia de los integrantes de diferentes grupos que participan en diversas actividades. Las actividades estarán agrupadas por categorías y la información podrá consultarse de acuerdo con diferentes rangos de fechas.

La aplicación permitirá registrar las organizaciones a las que pertenecen los grupos. Cada organización podrá contar con uno o varios grupos, y cada grupo tendrá un encargado que será seleccionado entre sus propios integrantes. Tanto el encargado como los integrantes deberán quedar registrados en el sistema con sus nombres, apellidos, dirección de residencia y número de teléfono.

También se contará con un apartado para registrar las categorías y las actividades. Cada actividad deberá estar asociada a una categoría y tendrá información como nombre, descripción, fecha, hora y lugar donde se realizará. De esta manera, las actividades podrán mantenerse organizadas y será más sencillo consultar posteriormente la información de asistencia.

Una de las funciones principales será el registro de asistencia. Para ello, el usuario podrá seleccionar una actividad y visualizar los integrantes correspondientes al grupo para indicar quiénes asistieron. Cada asistencia quedará almacenada en la base de datos SQLite, evitando que una misma persona pueda ser registrada más de una vez para una misma actividad.

La aplicación contará además con un sistema de consultas que permitirá conocer quiénes asistieron a una actividad determinada, cuántas veces asistió cada integrante a las actividades de una categoría específica y cuántas veces asistió cada integrante considerando todas las actividades. También será posible conocer cuántas personas participaron en cada categoría durante un período determinado.

Todas las consultas podrán realizarse mediante rangos de fechas específicos, permitiendo seleccionar una fecha inicial y una fecha final. También se podrán aplicar filtros por organización, grupo, integrante, categoría o actividad, con el objetivo de obtener información más precisa y facilitar el análisis de los registros.

La aplicación tendrá diferentes módulos, entre ellos una pantalla principal, administración de organizaciones, grupos e integrantes, registro de categorías y actividades, registro de asistencias, consultas, reportes y configuración.
La pantalla principal permitirá acceder de manera sencilla a cada una de estas funciones.

El desarrollo del proyecto se realizará por etapas. Primero se analizarán los requisitos y se diseñará la estructura de la aplicación y de la base de datos.
 
Posteriormente se configurará el proyecto utilizando C#, Blazor y .NET MAUI, además de implementar SQLite para almacenar la información de manera local. Después se desarrollarán los módulos de registro y administración de organizaciones, grupos, integrantes, categorías y actividades.

Una vez terminados los registros principales, se implementará el módulo de asistencia y posteriormente el sistema de consultas y reportes. Finalmente, se realizarán diferentes pruebas para comprobar que la información se registre correctamente, que no existan datos duplicados y que las consultas por fechas, categorías, actividades, grupos e integrantes proporcionen resultados correctos.

El resultado esperado es una aplicación sencilla, organizada y funcional que permita llevar un control completo de la asistencia de los integrantes, facilitando la consulta de quiénes participaron en determinadas actividades, cuántas veces asistieron, qué categorías tuvieron mayor participación y cómo fue la asistencia durante un rango de fechas específico.

