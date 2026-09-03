# Cuestionario: Marco de Trabajo .NET MAUI

**Nombre del entrevistado:** Daniela Alejandra López de León 

**Fecha:** 3 de septiembre

**Nivel de experiencia:** Principiante

---

## Sección A — Conocimientos generales

1. ¿Qué significa la sigla MAUI y qué es .NET MAUI?
MAUI significa **Multi-platform App UI**. Es un **framework de .NET** para crear aplicaciones multiplataforma.

2. ¿Quién desarrolló .NET MAUI y en qué año se lanzó oficialmente?
Fue desarrollado por **Microsoft** y se lanzó oficialmente en 2022.

3. ¿De qué marco de trabajo anterior es MAUI el sucesor? ¿Por qué se creó MAUI como reemplazo?
Es sucesor de **Xamarin.Forms** y se creó para ofrecer una solución multiplataforma más integrada con .NET.

4. ¿Qué plataformas o sistemas operativos permite targetear una aplicación desarrollada con MAUI?
**Android, iOS, macOS y Windows**.

5. ¿Qué lenguaje de programación se utiliza principalmente para desarrollar con .NET MAUI?
Principalmente Csharp, junto con XAML para las interfaces.

## Sección B — Arquitectura y estructura

6. ¿Qué es un proyecto .NET MAUI y cómo se estructura? Menciona las carpetas o archivos principales que encontrarías al crear uno nuevo.
Es un proyecto para crear aplicaciones multiplataforma. Incluye archivos como **MauiProgram.cs, App.xaml y AppShell.xaml**, además de carpetas de recursos y plataformas.

7. ¿Qué es el archivo `MauiProgram.cs` y qué función cumple?
Es el archivo donde se configura e inicia la aplicación MAUI.

8. ¿Qué es el archivo `App.xaml` / `App.xaml.cs` y cuál es su rol en la aplicación?
Contienen recursos y la configuración principal de la aplicación.

9. ¿Qué es el archivo `AppShell.xaml` y para qué sirve?
Define la estructura y navegación principal de la aplicación.

10. ¿Qué son las plataformas específicas (*Platforms* folder) dentro de un proyecto MAUI y qué contiene cada una?
Son carpetas con código necesario para adaptar la aplicación a **Android, iOS, macOS y Windows**.

## Sección C — Interfaz y componentes

11. ¿Qué es XAML y cómo se utiliza en .NET MAUI?
Es un lenguaje basado en XML utilizado para diseñar interfaces gráficas en MAUI.

12. ¿Cuál es la diferencia entre escribir la interfaz en XAML y escribirla directamente en C#?
**XAML** organiza visualmente la interfaz, mientras C# permite crear la interfaz y controlar su comportamiento mediante código.

13. Menciona al menos cinco controles (elementos de UI) disponibles en .NET MAUI.
***Button, Label, Entry, Image y CheckBox***.

14. ¿Qué es un `Layout` en MAUI? Menciona al menos tres tipos de layout y explica cuándo usarías cada uno.
Es un elemento que organiza los controles. Ejemplos: Grid para filas y columnas, VerticalStackLayout para elementos verticales y HorizontalStackLayout para elementos horizontales.

15. ¿Qué es el *data binding* (enlace de datos) en MAUI? Escribe o describe un ejemplo sencillo.
Es la conexión entre un elemento de la interfaz y una variable o propiedad.

16. ¿Qué es el patrón MVVM (*Model-View-ViewModel*) y por qué se recomienda usarlo en MAUI?
Es un patrón que separa la interfaz, los datos y la lógica, facilitando el mantenimiento de la aplicación.

## Sección D — Funcionalidades y servicios

17. ¿Qué es la inyección de dependencias (*Dependency Injection*) y cómo se configura en MAUI?
Permite que la aplicación reciba automáticamente los servicios que necesita.

18. ¿Qué es el *Shell Navigation* y cómo se define una ruta de navegación entre páginas?
Es el sistema de MAUI para navegar entre páginas y definir sus rutas.

19. ¿Cómo accede una aplicación MAUI a funcionalidades nativas del dispositivo como la cámara, el GPS o los sensores? ¿Qué es el patrón *Essentials*?
Mediante APIs de .NET MAUI que permiten utilizar funciones como GPS, cámara y sensores.

20. ¿Qué es .NET MAUI Essentials y menciona al menos tres servicios que ofrece?
Es el conjunto de APIs para acceder a funciones del dispositivo, como batería, conectividad y geolocalización.

21. ¿Cómo se manejan los recursos (imágenes, fuentes, estilos) de forma multiplataforma en MAUI?
Se colocan en carpetas como Resources y MAUI los adapta a las diferentes plataformas.

## Sección E — Comparación y contexto

22. ¿Cuál es la diferencia entre .NET MAUI y Xamarin.Forms?
MAUI es el sucesor de Xamarin.Forms y ofrece una integración más moderna con .NET.

23. ¿Cuál es la diferencia entre desarrollar una aplicación con MAUI y desarrollar una aplicación web con Blazor?
MAUI crea aplicaciones móviles y de escritorio, mientras Blazor se utiliza principalmente para aplicaciones web.

24. ¿Qué es .NET MAUI Blazor Hybrid y en qué caso lo utilizarías?
Permite usar componentes de Blazor dentro de aplicaciones MAUI. Es útil para reutilizar interfaces web en aplicaciones multiplataforma.

25. ¿Qué ventajas ofrece MAUI frente a frameworks como Flutter o React Native?
Permite utilizar Csharp y .NET, compartir código y acceder fácilmente a herramientas del ecosistema Microsoft.

26. ¿MAUI genera una aplicación nativa para cada plataforma o una aplicación web empaçada? Explica.
Genera aplicaciones nativas, utilizando controles y funciones propias de cada plataforma.


## Sección F — Herramientas y desarrollo

27. ¿Qué IDE o editor de código utilizarías para desarrollar con .NET MAUI?
Principalmente Visual Studio, aunque también se puede utilizar Visual Studio Code.

28. ¿Es necesario tener una Mac para desarrollar aplicaciones iOS con MAUI? Explica las opciones disponibles.
Para compilar aplicaciones iOS normalmente se necesita acceso a macOS, aunque se puede trabajar desde Windows usando un Mac remoto o conectado.

29. ¿Qué es Hot Reload en el contexto de MAUI y por qué es útil durante el desarrollo?
Permite ver cambios en la aplicación sin tener que reiniciarla completamente, facilitando el desarrollo.

30. ¿Cómo se compila y ejecuta una aplicación MAUI en un dispositivo Android durante el desarrollo?
Se puede ejecutar mediante un emulador de Android o un dispositivo físico, desde Visual Studio.


## Sección G — Pregunta reflexiva

31. ¿Crees que .NET MAUI es una buena opción para desarrolladores que ya conocen C# y quieren crear aplicaciones móviles y de escritorio? ¿Por qué? ¿Qué limitaciones o desafíos anticipas?

Sí, porque permite aprovechar Csharp y .NET para crear aplicaciones móviles y de escritorio. Una limitación es que algunas funciones específicas pueden requerir conocimientos de cada plataforma.
