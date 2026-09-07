# Cuestionario: Motor de Base de Datos SQLite

**Nombre del entrevistado:** Daniela Alejandra lópez de león 

**Fecha:** 7 de septiembre 
**Nivel de experiencia:** Principiante

---

## Sección A — Conocimientos generales

1. ¿Qué es SQLite y quién lo desarrolló?

SQLite es un motor de base de datos relacional, ligero y de código abierto. Fue desarrollado por D. Richard Hipp.

2. ¿En qué año aproximadamente se creó SQLite y cuál fue su objetivo principal?

Fue creado alrededor del año 2000. Su objetivo era proporcionar una base de datos sencilla, pequeña y que no necesitara un servidor.

3. ¿Qué significa que SQLite sea una base de datos **embebida** (*embedded*)?

Significa que la base de datos se integra directamente dentro de la aplicación y no necesita un servidor externo.

4. ¿SQLite es un sistema de gestión de bases de datos relacional (RDBMS) o no relacional? Justifica tu respuesta.

Es una base de datos relacional (RDBMS) porque organiza la información en tablas que pueden relacionarse entre sí y utiliza SQL.

5. ¿Cuál es la diferencia fundamental entre SQLite y sistemas como MySQL, PostgreSQL o SQL Server?

SQLite funciona directamente dentro de la aplicación y no necesita un servidor, mientras que los otros normalmente utilizan una arquitectura cliente-servidor.

6. ¿SQLite requiere un servidor para funcionar? Explica por qué.

No. SQLite es serverless, por lo que funciona directamente leyendo y escribiendo en un archivo de base de datos.

## Sección B — Características y arquitectura

7. ¿Cómo se almacenan los datos en SQLite? ¿Utiliza archivos o mantiene todo en memoria?

Los datos normalmente se almacenan en un archivo de la computadora, aunque SQLite también utiliza memoria durante su funcionamiento.

8. ¿Qué extensión de archivo tiene normalmente una base de datos SQLite?

Normalmente utiliza la extensión .db o .sqlite.

9. ¿Qué significa que SQLite sea **serverless** (sin servidor)?

Significa que no necesita un programa servidor independiente para administrar la base de datos.

10. ¿Qué significa que SQLite use **tipado dinámico** (*type affinity*) en lugar de tipado estricto como otros motores SQL?

Significa que los datos tienen flexibilidad en cuanto al tipo de valor que pueden almacenar, aunque las columnas tienen una afinidad de tipo.

11. ¿SQLite soporta transacciones? ¿Qué propiedades ACID cumple? Explica cada una brevemente.

Sí, SQLite soporta transacciones y cumple ACID:

Atomicidad: una operación se completa o no se realiza.
Consistencia: mantiene los datos correctos.
Aislamiento: las operaciones no interfieren incorrectamente entre sí.
Durabilidad: los cambios confirmados permanecen guardados.

12. ¿Cuáles son las limitaciones principales de SQLite frente a motores de bases de datos cliente-servidor?

No es la mejor opción para sistemas con muchos usuarios escribiendo al mismo tiempo, grandes aplicaciones distribuidas o necesidades avanzadas de un servidor.

## Sección C — SQL básico en SQLite

13. ¿Qué es SQL y cuál es su relación con SQLite?

SQL es un lenguaje utilizado para administrar bases de datos. SQLite utiliza SQL para crear, consultar y modificar sus datos.

14. ¿Cómo se crea una base de datos nueva en SQLite desde la línea de comandos?

sqlite3 escuela.db

Si el archivo no existe, SQLite lo crea.

15. Escribe la sentencia SQL para crear una tabla llamada `Estudiantes` con los campos: `Id` (entero, clave primaria), `Nombre` (texto), `Edad` (entero) y `Correo` (texto).

CREATE TABLE Estudiantes (
    Id INTEGER PRIMARY KEY,
    Nombre TEXT,
    Edad INTEGER,
    Correo TEXT
);

16. Escribe la sentencia SQL para insertar un registro en la tabla `Estudiantes`.

INSERT INTO Estudiantes (Nombre, Edad, Correo)
VALUES ('Daniela', 17, 'daniela@gmail.com');

17. Escribe la sentencia SQL para consultar todos los registros de la tabla `Estudiantes` donde la edad sea mayor a 18.

SELECT * FROM Estudiantes
WHERE Edad > 18;

18. ¿Cuál es la diferencia entre `DELETE` y `DROP TABLE`?

DELETE elimina registros de una tabla, mientras que DROP TABLE elimina la tabla completa.

19. ¿Qué es una clave primaria (*PRIMARY KEY*) y por qué es importante?

Es un campo que identifica de manera única cada registro de una tabla. Es importante para evitar confusiones y facilitar las relaciones.

20. ¿Qué es una clave foránea (*FOREIGN KEY*)? SQLite soporta claves foráneas por defecto o hay que activarlas. ¿Sabes cómo?

Es un campo que relaciona una tabla con otra. En SQLite se recomienda activarlas con:

PRAGMA foreign_keys = ON;

## Sección D — Operaciones y conceptos intermedios

21. ¿Qué es el comando `.tables` en el intérprete de línea de comandos de SQLite?

Es un comando de SQLite que muestra las tablas existentes en la base de datos.

22. ¿Qué es el comando `.schema` y para qué sirve?

Muestra la estructura de las tablas y otros objetos de la base de datos.

23. ¿Cómo se actualiza un registro existente en una tabla? Escribe un ejemplo.

UPDATE Estudiantes
SET Edad = 18
WHERE Id = 1;

24. ¿Qué son los índices (*INDEX*) en SQLite y cuándo son útiles?

Son estructuras que ayudan a buscar información más rápidamente. Son útiles cuando una tabla tiene muchos datos.

25. ¿Qué es una consulta `JOIN`? Describe con un ejemplo sencillo la diferencia entre `INNER JOIN` y `LEFT JOIN`.

Es una operación que permite combinar información de dos o más tablas relacionadas.

INNER JOIN: muestra solamente los registros que coinciden en ambas tablas.
LEFT JOIN: muestra todos los registros de la tabla izquierda, aunque no tengan coincidencia.

26. ¿Qué es `AUTOINCREMENT` en SQLite y cómo funciona? ¿Es igual que en otros motores de bases de datos?

Permite que SQLite genere automáticamente números para una columna de tipo entero. Se utiliza principalmente con claves primarias. No funciona exactamente igual que mecanismos similares de otros motores.

## Sección E — Uso práctico en el ecosistema de desarrollo

27. ¿Has utilizado SQLite dentro de alguna aplicación? Si es así, describe con qué tecnología o lenguaje.

SQLite puede utilizarse en aplicaciones desarrolladas con lenguajes como C#, Java, Python y JavaScript, entre otros.

28. ¿Cómo se integra SQLite en una aplicación .NET (C#, MAUI o Blazor)? ¿Conoces alguna librería o ORM para ello?

Se puede integrar mediante librerías como Microsoft.Data.Sqlite o utilizando herramientas como Entity Framework Core.

29. ¿Qué es un ORM (*Object-Relational Mapping*)? ¿Has oído hablar de Entity Framework o Dapper en relación con SQLite?

Es una herramienta que permite trabajar con bases de datos utilizando objetos del lenguaje de programación. Entity Framework es un ejemplo de ORM.

30. ¿En qué tipo de proyectos o situaciones considerarías que SQLite es la mejor opción?

Es ideal para aplicaciones pequeñas, aplicaciones móviles, programas de escritorio, proyectos educativos y aplicaciones que necesitan una base de datos local.

31. ¿SQLite es adecuado para aplicaciones web con miles de usuarios concurrentes? Justifica tu respuesta.

Generalmente no es la mejor opción, especialmente cuando muchos usuarios necesitan escribir datos al mismo tiempo. Para esos casos suelen ser mejores sistemas cliente-servidor.

## Sección F — Herramientas y exploración

32. ¿Conoces alguna herramienta gráfica (GUI) para administrar bases de datos SQLite? Menciona al menos una.

Sí. Una herramienta conocida es DB Browser for SQLite.

33. ¿Puedes abrir y explorar un archivo de base de datos SQLite con un editor de texto común? ¿Por qué sí o por qué no?

No de forma útil, porque el archivo de SQLite utiliza un formato binario, no texto normal.

34. ¿SQLite se puede usar desde la línea de comandos? ¿Qué comando ejecutarías para abrir una base de datos existente?

Sí. Para abrir una base de datos existente se puede utilizar:

sqlite3 nombre_base.db

## Sección G — Pregunta reflexiva

35. ¿Por qué crees que SQLite es uno de los motores de bases de datos más utilizados en el mundo a pesar de no ser un sistema cliente-servidor? ¿En qué situaciones lo considerarías ideal y en cuáles no?

Porque es ligero, gratuito, fácil de usar y no necesita un servidor. Es ideal para aplicaciones móviles, programas de escritorio y proyectos pequeños. No es la mejor opción cuando se necesitan muchos usuarios conectados simultáneamente o una infraestructura de servidor más avanzada.
