# Cuestionario: Marco de Trabajo Blazor

**Nombre del entrevistado:** Daniela Alejandra López de León
**Fecha:** 3/09/2026
**Nivel de experiencia:** Principiante

---

## Sección A — Conocimientos generales

1. ¿Qué es Blazor y quién lo desarrolló?
Blazor es un framework de desarrollo web creado por Microsoft y también fue desarrollado por Microsoft 

2. ¿Qué lenguaje de programación utiliza Blazor para crear interfaces web?
El lenguaje de programación principal de Blazor es Csharp 

3. ¿Qué significa que Blazor permite crear aplicaciones web con C# en lugar de JavaScript?
Blazor permite utilizar Csharp como lenguaje principal para desarrollar la lógica y los componentes de una aplicación web, en lugar de depender directamente de JavaScript   

4. ¿Cuál es la diferencia entre **Blazor Server** y **Blazor WebAssembly**?
Blazor Server ejecuta el código en el servidor, mientras que Blazor WebAssembly ejecuta el código directamente en el navegador.

5. ¿Qué es un componente en Blazor?
Parte reutilizable de una aplicación web que contiene su propia interfaz y lógica.

## Sección B — Conceptos fundamentales

6. ¿Qué extensión de archivo tienen los componentes de Blazor?
La extensión .razor


7. ¿Qué son los parámetros de componente (`[Parameter]`) en Blazor? Da un ejemplo.
Permiten pasar información de un componente a otro.

Ejemplo:

[Parameter]
public string Nombre { get; set; }


8. ¿Qué es el *data binding* (enlace de datos) en Blazor? Explica la diferencia entre *one-way binding* y *two-way binding*.
One-way: los datos van en una sola dirección.
Two-way: los datos se actualizan en ambas direcciones.


9. ¿Qué directiva usarías para enlazar dinámicamente el valor de un campo de texto con una variable? Escribe un ejemplo.
Se utiliza @bind.

<input @bind="nombre" />


10. ¿Qué son los *lifecycle methods* (métodos del ciclo de vida) de un componente? Menciona al menos dos.
Son métodos que se ejecutan en diferentes etapas de un componente, como al iniciarse o actualizarse.

## Sección C — Uso práctico

11. ¿Qué es `@page` en Blazor y para qué sirve?
Es una directiva que define la ruta de una página.

@page "/inicio"

12. ¿Cómo se navega entre páginas en una aplicación Blazor?
Mediante enlaces **<a>** o usando **NavigationManager**.

13. ¿Qué es la inyección de dependencias (`Dependency Injection`) y cómo se usa en Blazor?
Permite que un componente reciba los servicios que necesita automáticamente.

14. ¿Cómo se consumen servicios o APIs REST desde una aplicación Blazor?
Utilizando **HttpClient** para enviar solicitudes y recibir datos.

15. ¿Qué es `@inject` y cómo funciona?
Es una directiva que permite inyectar un servicio en un componente.

## Sección D — Comparación y contexto

16. ¿Qué ventajas ves en Blazor frente a frameworks como Angular, React o Vue?
Permite usar **Csharp** en lugar de **JavaScript** y se integra fácilmente con **.NET**.

17. ¿Blazor reemplaza completamente a JavaScript? Justifica tu respuesta.
No. **JavaScript** todavía es necesario para algunas funciones y bibliotecas.

18. ¿En qué tipo de proyecto considerarías que Blazor es una buena opción?
En aplicaciones empresariales, sistemas administrativos y proyectos **.NET**.

19. ¿Qué es MAUI Blazor y cómo se relaciona con Blazor?
Es la combinación de **.NET MAUI** y Blazor para crear aplicaciones multiplataforma.

20. ¿Has creado algún proyecto o ejemplo con Blazor? Si es así, descríbelo brevemente.
no

## Sección E — Pregunta reflexiva

21. ¿Crees que el ecosistema de Blazor tiene futuro para el desarrollo web profesional? ¿Por qué?
Sí, porque permite desarrollar aplicaciones web con **Cshap y .NET**, tecnologías muy utilizadas en proyectos profesionales.
