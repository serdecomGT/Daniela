# Cuestionario: Lenguaje de Programación C#

**Nombre del entrevistado:** Daniela Alejandra López de León 
**Fecha:** 3 de septiembre 
**Nivel de experiencia:** Principiante

---

## Sección A — Conocimientos generales

1. ¿Quién desarrolló el lenguaje C# y en qué año se lanzó oficialmente?
Fue desarrollado por **Microsoft**, liderado por **Anders Hejlsberg**, y se lanzó oficialmente en **2002**.

2. ¿C# es un lenguaje compilado, interpretado o ambos? Explica brevemente.Ç
Es principalmente compilado. El código se convierte en un lenguaje intermedio que luego ejecuta **.NET**.

3. ¿Qué significa que C# sea un lenguaje de tipado estático?
Significa que cada variable tiene un tipo definido, **como int, string o double**.

4. ¿Qué es el framework .NET y cuál es su relación con C#?
**.NET** es una plataforma para desarrollar aplicaciones. **Csharp** es uno de los principales lenguajes utilizados en ella.

5. Menciona al menos tres tipos de aplicaciones que se pueden desarrollar con C#.
Aplicaciones web, de escritorio y móviles.

## Sección B — Sintaxis y conceptos básicos

6. ¿Cómo se declara una variable de tipo entero en C#? Escribe un ejemplo.
**int edad = 18;**

7. ¿Cuál es la diferencia entre `var`, `int` y `string` al declarar una variable?
**int** almacena números enteros, **string** almacena texto y var permite que **Csharp** determine automáticamente el tipo.

8. ¿Qué diferencia hay entre `const` y `readonly`?
const no puede cambiar nunca. **readonly** puede asignarse durante la declaración o en el constructor.

9. Escribe un ejemplo de una estructura condicional `if-else` en C#.

Çif (edad >= 18)
{
    Console.WriteLine("Mayor de edad");
}
else
{
    Console.WriteLine("Menor de edad");
}

10. Escribe un ejemplo de un ciclo `for` que imprima los números del 1 al 5.

for (int i = 1; i <= 5; i++)
{
    Console.WriteLine(i);
}

11. ¿Qué es un método en C#? Escribe un ejemplo de un método que reciba dos números y devuelva su suma.

Es un bloque de código que realiza una tarea específica.

int Sumar(int a, int b)
{
    return a + b;
}

## Sección C — Programación Orientada a Objetos

12. ¿Qué es una clase en C#? Escribe un ejemplo básico.

Es un modelo o plantilla para crear objetos.

class Persona
{
    public string Nombre;
}

13. ¿Qué es un objeto y cómo se relaciona con una clase?

Es una instancia de una clase. La clase es el modelo y el objeto es algo creado a partir de ese modelo.

14. Explica con tus propias palabras los conceptos de **encapsulamiento**, **herencia** y **polimorfismo**.

Encapsulamiento: protege los datos de una clase.
Herencia: permite que una clase herede características de otra.
Polimorfismo: permite que un mismo método tenga diferentes comportamientos.

15. ¿Qué son los modificadores de acceso `public`, `private` y `protected`? ¿Cuándo usarías cada uno?

public: accesible desde cualquier lugar.
private: solo dentro de la clase.
protected: dentro de la clase y sus clases derivadas.

16. ¿Qué es un constructor y para qué sirve?

Es un método especial que se ejecuta al crear un objeto y sirve para inicializarlo.

## Sección D — Conceptos adicionales

17. ¿Qué es un `namespace` y por qué es útil?

Es una forma de organizar clases y evitar conflictos entre nombres.

18. ¿Qué son las excepciones en C#? ¿Cómo se manejan?

Son errores que pueden ocurrir durante la ejecución. Se manejan principalmente con **try, catch y finally**.

19. ¿Qué es LINQ y para qué se utiliza?

Es una herramienta de Csharp que permite consultar y organizar datos fácilmente.

20. ¿Conoces algún IDE o editor de código para programar en C#? ¿Cuál has utilizado?

No

## Sección E — Pregunta reflexiva

21. ¿En qué situaciones considerarías que C# es una buena elección frente a otros lenguajes como Python o Java?
Cshap es una buena opción para aplicaciones web, empresariales, de escritorio, videojuegos y proyectos que utilizan .NET.
