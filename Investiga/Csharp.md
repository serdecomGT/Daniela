# Csharp

---

## ¿Qué es Csharp?
Csharp es un lenguaje de programación moderno, orientado a objetos y desarrollado por Microsoft. Fue creado para desarrollar diferentes tipos de programas y actualmente forma parte del ecosistema .NET.

Sharp permite darle instrucciones a una computadora para realizar determinadas acciones. Con él se pueden crear desde programas sencillos hasta sistemas empresariales complejos, aplicaciones móviles, páginas web y videojuegos.

## ¿Cuál es su función?
La función principal de Csharp es permitir a los desarrolladores crear software mediante código.

El programador escribe instrucciones utilizando **la sintaxis de Csharp**, y posteriormente **.NET** se encarga de proporcionar el entorno necesario para que ese programa pueda ejecutarse.

Por ejemplo, con Csharp se puede indicar:

¿Qué información debe mostrar un programa.
. ¿Cómo debe responder cuando un usuario presiona un botón?
. Cómo guardar o consultar información.
. Cómo realizar cálculos.
. Cómo conectarse a una base de datos.
. Cómo comunicarse con otros servicios.
. Cómo controlar diferentes partes de una aplicación.

## ¿Qué se puede hacer con el Csharp?

Aplicaciones móviles
Mediante .NET MAUI, Csharp puede utilizarse para desarrollar aplicaciones destinadas a Android, iOS, Windows y macOS.

Aplicaciones web
Con ASP.NET Core, Csharp puede utilizarse para crear páginas web, APIs y aplicaciones web.

Videojuegos
Csharp es muy utilizado con Unity, un motor de desarrollo de videojuegos. Esto permite crear personajes, sistemas de juego, menús, movimientos y diferentes mecánicas.

Aplicaciones de escritorio
Puede utilizarse para crear programas que funcionan directamente en computadoras.

**Por ejemplo:**
Sistemas de inventario.
Sistemas escolares.
Programas administrativos.
Calculadoras.
Sistemas de ventas.

Servicios y aplicaciones en la nube
Csharp también puede utilizarse para desarrollar servicios que funcionan en servidores y se comunican mediante Internet.

Inteligencia artificial
El ecosistema .NET cuenta con herramientas y bibliotecas que permiten trabajar con inteligencia artificial, aprendizaje automático y procesamiento de datos.

## ¿Cómo funciona?
Un programa de Csharp está compuesto por instrucciones que indican qué debe hacer el sistema.

Por ejemplo:

int edad = 17;

if (edad >= 18)
{
    Console.WriteLine("Es mayor de edad");
}
else
{
    Console.WriteLine("Es menor de edad");
}

Aquí se crea una variable llamada **edad** y después se utiliza una condición **if** para determinar qué mensaje mostrar.

Esto demuestra que Csharp puede utilizar variables, condiciones, operaciones, métodos, clases y objetos para construir programas más complejos.Ç

## Caracteristicas completas 
**1. Orientado a objetos**
Csharp utiliza la programación orientada a objetos, un modelo que permite organizar el código mediante clases y objetos.

**2. Fuertemente tipado**
Las variables tienen un tipo definido, como:
int edad = 17;
string nombre = "Daniela";
bool activo = true;
Esto ayuda a detectar determinados errores durante el desarrollo.

**Multiplataforma**
Gracias a **.NET, Csharp** puede utilizarse para crear software destinado a diferentes sistemas operativos.

4. Reutilización de código
Permite crear componentes que pueden reutilizarse en diferentes partes de una aplicación.

5. Gran cantidad de bibliotecas
**.NET** proporciona numerosas herramientas que facilitan tareas como trabajar con archivos, bases de datos, redes, aplicaciones web y mucho más.

## Elementos básicos de Csharp
Para comenzar a programar en Csharp es importante conocer algunos conceptos:

Variables: almacenan información.
Tipos de datos: indican qué tipo de información se almacena.
Condicionales: permiten tomar decisiones.
Bucles: permiten repetir instrucciones.
Métodos: agrupan instrucciones para realizar determinadas tareas.
Clases: sirven como estructuras para crear objetos.
Objetos: representan elementos que contienen información y comportamientos.
Excepciones: permiten controlar determinados errores durante la ejecución.

## Datos curiosos de Csharp
Csharp fue desarrollado por Microsoft.
Su primera versión apareció en **2000**.
Su creador principal fue **Anders Hejlsberg**, quien también participó en el desarrollo de otros lenguajes y herramientas de programación.
Su nombre se pronuncia “C Sharp”.
El símbolo # se relaciona con el concepto musical C♯ (Do sostenido).
Csharp está estrechamente relacionado con **.NET.**
Es uno de los lenguajes más importantes utilizados dentro del **ecosistema de Microsoft.**
Se utiliza en videojuegos desarrollados con **Unity**.
Puede utilizarse tanto para proyectos pequeños como para sistemas empresariales de gran tamaño.
Csharp continúa recibiendo nuevas versiones y características.

## Ventajas de Csharp
Es versátil.
Tiene una sintaxis relativamente organizada.
Cuenta con muchas herramientas de desarrollo.
Está integrado con .NET.
Permite crear diferentes tipos de aplicaciones.
Tiene una gran cantidad de bibliotecas.
Puede utilizarse en múltiples plataformas.
Es utilizado profesionalmente en diferentes industrias.

## Desventajas de Csherp
Puede ser difícil para alguien que está comenzando desde cero.
Tiene muchos conceptos que aprender.
Los proyectos grandes pueden volverse complejos.
Para aprovechar todo su potencial es necesario conocer también partes del ecosistema .NET.

## Importancia de Csharp
Csharp es importante porque permite desarrollar una gran variedad de soluciones tecnológicas utilizando un lenguaje que puede adaptarse a diferentes necesidades. Su integración con .NET, su utilización en videojuegos y su capacidad para crear aplicaciones web, móviles y de escritorio lo convierten en una herramienta muy útil para los desarrolladores.

# Sintaxis
La sintaxis de Csharp está formada por las reglas que indican cómo deben escribirse las instrucciones para que el programa pueda entenderlas y ejecutarlas.
using System;

**1. Estructura básica**
class Programa
{
    static void Main()
    {
        Console.WriteLine("Hola mundo");
    }
}

. using System; permite utilizar elementos de la biblioteca System.
. class Programa crea una clase llamada Programa.
. static void Main() es el punto donde comienza la ejecución del programa.
. Console.WriteLine() muestra información en la pantalla.
. { } delimitan bloques de código.
. ; indica el final de una instrucción.

**2. Variables**
Las variables almacenan información:

int edad = 17;
string nombre = "Carlos";
double promedio = 85.5;
bool aprobado = true;

**3. Condicionales**
Permiten tomar decisiones:

if (edad >= 18)
{
    Console.WriteLine("Es mayor de edad");
}
else
{
    Console.WriteLine("Es menor de edad");
}


**4. Ciclos**
Permiten repetir instrucciones:

for (int i = 1; i <= 5; i++)
{
    Console.WriteLine(i);
}


**5. Métodos**
Los métodos agrupan instrucciones que realizan una determinada tarea:

static void Saludar()
{
    Console.WriteLine("Hola");
}

Después pueden llamarse desde otra parte del programa:

Saludar();


**6. Clases y objetos**
Csharp utiliza ampliamente la programación orientada a objetos:

class Estudiante
{
    public string nombre;
    public int edad;
}

Después se puede crear un objeto:

Estudiante alumno = new Estudiante();
alumno.nombre = "Carlos";
alumno.edad = 17;

# Reglas importantes de la sintaxis
Las instrucciones normalmente terminan con ;.
Las llaves { } delimitan bloques de código.
Csharp distingue entre mayúsculas y minúsculas.
Los comentarios de una línea comienzan con //.
Los comentarios de varias líneas pueden escribirse entre /* y */.
Las palabras reservadas, como if, class, int y for, tienen funciones específicas dentro del lenguaje.

# Conclusión
Csharp es un lenguaje de programación completo y versátil que permite desarrollar diferentes tipos de aplicaciones. Su integración con .NET facilita la creación de programas web, móviles, de escritorio y videojuegos, por lo que se ha convertido en una herramienta importante dentro del desarrollo de software.
