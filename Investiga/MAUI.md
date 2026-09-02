# MAUI
---

##  ¿Qué significa MAUI?

MAUI significa ***Multi-platform App UI***, que en español puede entenderse como Interfaz de Usuario de Aplicaciones Multiplataforma.

Es un framework de código abierto de Microsoft que permite crear aplicaciones móviles y de escritorio nativas utilizando principalmente Csharp y XAML. Su característica principal es que permite trabajar con una base de código compartida para diferentes plataformas.

Actualmente ***.NET MAUI** permite desarrollar aplicaciones para Android, iOS, macOS y Windows; la documentación actual también contempla Tizen en determinados escenarios.

## ¿Cuál es el objetivo de .NET MAUI?
Su objetivo principal es simplificar el desarrollo multiplataforma.

Antes, desarrollar una aplicación para diferentes sistemas podía significar mantener proyectos y códigos separados. MAUI busca que el desarrollador pueda compartir tanto como sea posible:

Código.
Lógica de negocio.
Interfaz.
Recursos.
Pruebas.
Configuraciones.

Microsoft señala que uno de los objetivos principales de MAUI es implementar la mayor cantidad posible de la lógica y el diseño de una aplicación en una única base de código.

## ¿Cómo funciona?

Podemos imaginarlo de esta manera:

Programador =
Csharp + XAML=
.NET MAUI=
APIs de cada plataforma=

Android - iOS - Windows - macOS

MAUI proporciona una capa común que permite trabajar con elementos de la aplicación y, al mismo tiempo, acceder a características específicas del sistema cuando es necesario.

Csharp y MAUI

Csharp se utiliza principalmente para programar el comportamiento de la aplicación.
Por ejemplo, podemos tener un botón que, cuando el usuario lo presiona, realiza una determinada operación.

private void OnButtonClicked(object sender, EventArgs e)
{
    DisplayAlert("Mensaje", "Hola mundo", "OK");
}

Aquí Csharp se encarga de definir qué sucede cuando ocurre una acción.

**XAML y MAUI**

XAML puede utilizarse para definir la parte visual de una aplicación.

Por ejemplo:

<VerticalStackLayout>
    <Label
        Text="Bienvenido"
        FontSize="30" />

    <Button
        Text="Presionar" />
</VerticalStackLayout>

XAML permite organizar elementos visuales como:

Botones.
Textos.
Imágenes.
Listas.
Campos de entrada.
Diseños.
Menús.

Microsoft explica que XAML se utiliza principalmente para definir el contenido visual de las páginas y trabaja junto con archivos de Csharp.

Interfaces gráficas
.NET MAUI proporciona diferentes controles para construir interfaces.

Algunos ejemplos son:

Label
Muestra texto.
Button
Permite realizar una acción.
Entry
Permite introducir información.
Image
Muestra imágenes.
CollectionView
Permite presentar colecciones de datos.
CheckBox
Permite seleccionar o deseleccionar una opción.
Switch
Permite activar o desactivar una opción.

Estos componentes pueden combinarse para construir interfaces completas.

##  Organización de la interfaz

MAUI también proporciona diferentes herramientas para organizar los elementos visuales.

Por ejemplo:

VerticalStackLayout
HorizontalStackLayout
Grid
ScrollView

Esto permite decidir cómo se acomodarán los elementos en la pantalla.

Por ejemplo:

<VerticalStackLayout>
    <Label Text="Nombre:" />
    <Entry Placeholder="Escribe tu nombre" />
    <Button Text="Guardar" />
</VerticalStackLayout>

En este ejemplo, los elementos aparecen organizados verticalmente.


## Acceso a funciones del dispositivo

Esta parte es bastante interesante.

.NET MAUI puede proporcionar APIs multiplataforma para acceder a determinadas funciones del dispositivo, como:

GPS.
Estado de conexión.
Información de batería.
Sensores.
Brújula.
Información del dispositivo.
Archivos.
Texto a voz.
Tortapapeles.

Microsoft documenta estas capacidades como parte de la integración de MAUI con las características de cada plataforma.

MAUI y servicios web

Una aplicación MAUI también puede comunicarse con servidores mediante servicios web.

Por ejemplo:
Aplicación MAUI=
API=
Servidor=
Base de datos

La aplicación podría solicitar información de estudiantes, productos, usuarios o cualquier otro tipo de datos.

Microsoft incluye entre las tareas habituales de MAUI el consumo de servicios web REST mediante tecnologías como HTTP y JSON.
MAUI y bases de datos

También se pueden crear aplicaciones que trabajen con información almacenada localmente o en servidores.

Por ejemplo, una aplicación escolar podría guardar:
Nombre
Edad
Grado
Curso
Promedio

Y después permitir:

Agregar estudiantes.
Modificar información.
Buscar estudiantes.
Eliminar registros.
Consultar datos.

Esto hace que MAUI sea útil para crear sistemas administrativos.

**MAUI y MVVM**

En aplicaciones más grandes se puede utilizar el patrón MVVM (Model-View-ViewModel).

Sus partes principales son:

Model = datos y estructuras
View = interfaz visual
ViewModel = lógica que conecta la interfaz con los datos
Una representación sencilla sería:
Usuario = View = ViewModel = Model

Este patrón ayuda a separar responsabilidades y facilita el mantenimiento del proyecto. Microsoft utiliza MVVM como uno de los patrones recomendados para aplicaciones MAUI más estructuradas.

Hot Reload

Una función bastante interesante es .NET Hot Reload.

Permite realizar determinados cambios en el código mientras la aplicación está ejecutándose y observar los resultados sin tener que reconstruir manualmente todo el proyecto.

También existe XAML Hot Reload, que permite modificar la interfaz y observar los cambios rápidamente.

Esto resulta especialmente útil cuando se está diseñando una interfaz.

MAUI Community Toolkit

Existe además el .NET MAUI Community Toolkit, una colección de elementos reutilizables que proporciona herramientas adicionales para desarrollar aplicaciones.

Incluye recursos relacionados con:

Animaciones.
Comportamientos.
Convertidores.
Efectos.
Ayudantes.

Esto puede facilitar determinadas tareas de desarrollo.

## Historia de MAUI

.NET MAUI es la evolución de **Xamarin.Forms**.

Xamarin.Forms permitió desarrollar interfaces multiplataforma, principalmente para escenarios **móviles**. MAUI amplió este concepto para incluir también aplicaciones de escritorio y lo integró dentro del ecosistema moderno de .NET.

Por eso, alguien que ya conozca Xamarin.Forms puede encontrar conceptos familiares al aprender MAUI.

¿Qué es lo más interesante de MAUI?

Una de sus características más interesantes es que permite combinar desarrollo multiplataforma con acceso a funciones nativas.

Es decir, no tienes que elegir entre:

"Código compartido"
o
"Características específicas del dispositivo".

Puedes tener código compartido para la mayor parte de la aplicación y, cuando sea necesario, utilizar APIs específicas de Android, iOS, Windows o macOS.

Datos curiosos
MAUI significa Multi-platform App UI.
Es un proyecto de código abierto.
Es desarrollado dentro del ecosistema de Microsoft.
Es la evolución de Xamarin.Forms.
Utiliza principalmente C# y XAML.
Permite crear aplicaciones móviles y de escritorio.
Utiliza un sistema de proyecto único.
Puede acceder a características del dispositivo.
Permite compartir código entre plataformas.
Cuenta con herramientas como Hot Reload.
Tiene un Community Toolkit con componentes reutilizables.

### Ventajas

1. Desarrollo multiplataforma: permite trabajar con varias plataformas desde un mismo proyecto.
2. Código reutilizable: se puede compartir gran parte de la lógica y la interfaz.
3. Integración con C#: resulta especialmente útil para quienes ya conocen C#.
4. Integración con .NET: puede aprovechar bibliotecas y herramientas del ecosistema.
5. Acceso a funciones nativas: permite trabajar con características específicas de los dispositivos.
6. Mantenimiento: compartir código puede reducir la cantidad de partes que deben mantenerse por separado.

### Desventajas
Puede tener una curva de aprendizaje considerable para principiantes.
No todo el código puede compartirse entre plataformas.
Algunas características requieren conocimientos específicos del sistema operativo.
Las aplicaciones grandes necesitan una arquitectura y organización adecuadas.
Para desarrollar determinadas aplicaciones de Apple se necesita el entorno correspondiente de Apple; Microsoft señala específicamente que la compilación para iOS y macOS requiere un Mac.

## Conclusión

.NET MAUI es una tecnología diseñada para facilitar la creación de aplicaciones móviles y de escritorio multiplataforma. Su capacidad para compartir código, utilizar Csharp y XAML, acceder a funciones de los dispositivos y trabajar con servicios web y bases de datos lo convierte en una herramienta muy completa. Además, su sistema de proyecto único y características como Hot Reload ayudan a simplificar el desarrollo. Aunque requiere conocimientos de programación y algunas funciones necesitan código específico para cada plataforma, MAUI representa una alternativa interesante para desarrollar aplicaciones modernas utilizando el ecosistema .NET.
