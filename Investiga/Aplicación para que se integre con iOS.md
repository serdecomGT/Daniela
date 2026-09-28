# INFORME SOBRE LAS LIMITACIONES PARA UTILIZAR ASISGRU EN DISPOSITIVOS iOS

## 1. Introducción

Durante el desarrollo de la aplicación móvil **ASISGRU**, se trabajó en la creación de un sistema destinado al control y registro de asistencia de los integrantes de diferentes tipos de grupos. La aplicación fue desarrollada utilizando herramientas como **CSharp**, **.NET 10**, **.NET MAUI**, **Blazor**, **Visual Studio 2026** y **SQLite** como sistema de almacenamiento local.

El proyecto fue desarrollado principalmente desde un equipo con sistema operativo Windows, debido a que este fue el entorno disponible durante el proceso de práctica supervisada. Dentro de este entorno fue posible desarrollar, modificar, probar y ejecutar la aplicación para dispositivos Android. Sin embargo, al intentar considerar la posibilidad de utilizar la misma aplicación en dispositivos iPhone, se presentó una limitación importante relacionada con el proceso de desarrollo para el sistema operativo iOS.

La principal dificultad no se encuentra necesariamente en el código de ASISGRU ni significa que la aplicación no pueda ser desarrollada para iPhone. El inconveniente se relaciona con los requisitos específicos establecidos por Apple para la creación, compilación, firma y distribución de aplicaciones destinadas a iOS.

.NET MAUI permite crear aplicaciones multiplataforma a partir de una misma base de código. Esto significa que un proyecto desarrollado con .NET MAUI puede tener como objetivo diferentes plataformas, incluyendo Android e iOS. Sin embargo, cada plataforma tiene requisitos propios. En el caso de iOS, las herramientas de compilación de Apple requieren un entorno Mac.

Microsoft establece que para compilar aplicaciones nativas de iOS utilizando .NET MAUI es necesario tener acceso a las herramientas de compilación de Apple, las cuales funcionan en un equipo Mac. Por esta razón, cuando el desarrollo se realiza desde Windows, Visual Studio debe conectarse a un equipo Mac que pueda utilizarse como equipo de compilación.

Por lo anterior, el objetivo de este informe es explicar de manera detallada por qué ASISGRU no puede ser compilada y utilizada directamente en un iPhone desde el entorno actual de desarrollo en Windows, cuáles son los requisitos que intervienen en el proceso y qué alternativas existen para continuar trabajando en el proyecto.

---

## 2. Desarrollo de la aplicación ASISGRU

ASISGRU fue concebida como una aplicación móvil para el control y registro de asistencia de integrantes de grupos comunitarios, religiosos, deportivos, culturales, educativos y de otros tipos.

Durante su desarrollo se utilizaron diferentes tecnologías. El lenguaje principal utilizado fue **C#**, mientras que el marco de desarrollo fue **.NET 10**, utilizando **.NET MAUI y Blazor** para la construcción de la aplicación móvil. Para almacenar la información se utilizó **SQLite**, permitiendo mantener los datos de manera local en el dispositivo.

La aplicación cuenta con diferentes módulos relacionados con la configuración del grupo, administración de participantes, categorías, actividades y registro de asistencia. Estos componentes fueron desarrollados y probados dentro del entorno disponible durante la práctica.

El desarrollo realizado en Windows permitió trabajar principalmente con Android. Microsoft indica que Windows permite desarrollar y compilar aplicaciones .NET MAUI para Windows y Android. Sin embargo, para desarrollar y compilar la versión destinada a iOS se necesita acceso a un Mac debido a las herramientas específicas de Apple.

Esto permite comprender una diferencia importante: **desarrollar una aplicación multiplataforma no significa que todas las plataformas puedan ser compiladas desde cualquier sistema operativo**.

.NET MAUI facilita que gran parte del código de una aplicación pueda ser compartido entre diferentes plataformas, pero cada sistema operativo mantiene requisitos propios para generar la aplicación final.

En el caso de Android, las herramientas necesarias pueden instalarse y utilizarse directamente en Windows. En cambio, para iOS se necesitan herramientas proporcionadas por Apple, principalmente Xcode, que solamente puede ejecutarse en macOS.

Por lo tanto, ASISGRU no necesita ser reconstruida completamente para poder llegar a iPhone. El proyecto puede continuar utilizando gran parte del trabajo realizado. La dificultad principal consiste en disponer del entorno necesario para generar y firmar la versión de iOS.

---

## 3. ¿Por qué no se puede compilar directamente para iPhone desde Windows?

Una de las principales razones por las cuales ASISGRU no puede convertirse directamente en una aplicación para iPhone desde el equipo Windows utilizado durante el desarrollo es que **Apple requiere herramientas específicas para generar aplicaciones destinadas a sus dispositivos**.

Para compilar una aplicación nativa para iOS se utilizan herramientas de Apple incluidas dentro de **Xcode**. Estas herramientas son necesarias para diferentes procesos relacionados con la compilación, firma y preparación de la aplicación.


Microsoft explica que la compilación de aplicaciones nativas de iOS mediante .NET MAUI requiere acceso a las herramientas de compilación de Apple, las cuales solamente funcionan en Mac.

Esto significa que instalar .NET MAUI, C#, Visual Studio y el resto de las herramientas de desarrollo en Windows no es suficiente para producir directamente una aplicación iOS.

El problema puede explicarse de una manera sencilla:

**Windows → permite desarrollar y compilar para Android.**

**Mac → permite acceder a las herramientas necesarias para compilar para iOS.**

Por esta razón, una persona puede escribir y modificar el código de una aplicación .NET MAUI desde Windows, pero cuando llega el momento de crear la versión nativa para iPhone, necesita utilizar un equipo Mac como parte del proceso.

Esta característica no es una limitación exclusiva de ASISGRU. Es una condición relacionada con el proceso de desarrollo para la plataforma iOS.

Visual Studio ofrece una herramienta denominada **Pair to Mac**, que permite conectar el equipo Windows con un Mac disponible en la red. De esta manera, el desarrollador puede continuar trabajando desde Windows mientras el Mac se encarga de utilizar las herramientas de Apple necesarias para la compilación.

El funcionamiento puede representarse de la siguiente manera:

**Equipo Windows**
**Visual Studio**
**Conexión con Mac**
**Xcode y herramientas de Apple**
**Compilación de ASISGRU para iOS**
**Aplicación destinada al iPhone**

Por lo tanto, el hecho de no disponer actualmente de un Mac no significa que el proyecto esté perdido o que deba comenzar nuevamente desde cero. Significa que el proceso de compilación para iOS no puede completarse utilizando únicamente el equipo Windows.

---

# 4. Importancia de Xcode en el desarrollo para iOS

Uno de los elementos principales que hace falta para generar una versión de ASISGRU para iPhone es **Xcode**.

Xcode es el entorno de desarrollo proporcionado por Apple para sus plataformas. Dentro de él se encuentran las herramientas necesarias para construir aplicaciones destinadas a los sistemas operativos de Apple.

En el caso de .NET MAUI, Microsoft señala que el equipo Mac utilizado como host de compilación debe contar con Xcode instalado. Además, Xcode debe abrirse después de su instalación para completar la configuración correspondiente.

Un aspecto importante es que la función **Pair to Mac** de Visual Studio puede configurar automáticamente diferentes componentes necesarios en el Mac, pero **no instala Xcode**. Xcode debe instalarse directamente en el Mac.

Por esta razón, si solamente se dispone de un equipo Windows, no es posible instalar Xcode de manera normal en ese equipo para utilizarlo como si fuera una herramienta de Windows.

Esta situación explica una de las principales razones por las cuales ASISGRU puede ejecutarse en Android durante el desarrollo actual, pero no puede ser compilada de la misma manera para un iPhone.

También se debe considerar que el desarrollo de aplicaciones para iOS no termina simplemente con generar el archivo de la aplicación. Apple requiere procesos relacionados con la firma y la autorización de las aplicaciones.

Microsoft indica que para compilar, firmar e implementar aplicaciones .NET MAUI para iOS se requiere un equipo Mac compatible con Xcode. También se requiere un Apple ID y, para determinados procesos de implementación y publicación, una inscripción al Apple Developer Program.

Por lo tanto, existen varias etapas que deben cumplirse antes de poder utilizar ASISGRU en un iPhone de manera adecuada.

---

# 5. Diferencia entre desarrollar en Windows y publicar para iPhone

Es importante diferenciar entre **programar la aplicación** y **compilar, firmar y distribuir la aplicación**.

El código de ASISGRU puede continuar desarrollándose desde Windows. Es posible modificar las páginas, corregir errores, agregar funciones, cambiar el diseño y trabajar sobre la lógica de la aplicación sin tener necesariamente un Mac.

Sin embargo, cuando se desea generar la versión destinada a iOS, aparece el requisito del equipo Mac.

Microsoft proporciona precisamente el sistema denominado **Pair to Mac**, mediante el cual Visual Studio instalado en Windows puede conectarse a un Mac disponible en la red. Visual Studio envía el trabajo al Mac y utiliza las herramientas de Apple que se encuentran instaladas allí.

Esto permite mantener Windows como el equipo principal de desarrollo.

Por ejemplo, el flujo de trabajo podría ser:

1. Se abre ASISGRU en Visual Studio desde Windows.
2. Se realizan modificaciones en el código.
3. Se selecciona el objetivo iOS.
4. Visual Studio se conecta al Mac.
5. El Mac utiliza Xcode y las herramientas correspondientes.
6. Se compila la aplicación.
7. Se realizan los procesos de firma correspondientes.
8. Se obtiene una versión que puede utilizarse para pruebas o distribución, dependiendo de la configuración y las cuentas disponibles.

Microsoft también documenta la posibilidad de realizar compilaciones de aplicaciones iOS desde la línea de comandos de Windows cuando existe un Mac configurado como equipo de compilación remoto.

Por lo tanto, **no es obligatorio que todo el trabajo se realice físicamente en un Mac**. Lo que sí es necesario es tener acceso a un Mac que pueda realizar la parte del proceso que depende de las herramientas de Apple.

---

# 6. Requisitos adicionales para probar ASISGRU en un iPhone

Otro aspecto importante es la diferencia entre compilar la aplicación y probarla en un dispositivo físico.

Un simulador puede ser utilizado para realizar determinadas pruebas durante el desarrollo, pero Microsoft recomienda realizar también pruebas en un dispositivo físico, debido a que algunos problemas pueden aparecer solamente en el hardware real.

Para instalar y probar una aplicación iOS en un iPhone se deben considerar procesos de **provisioning**, firma y configuración de Apple.

Microsoft señala que para compilar, firmar e implementar aplicaciones .NET MAUI para iOS se necesita un equipo Mac compatible con Xcode, además de un Apple ID y, para determinadas formas de implementación, una suscripción de pago al Apple Developer Program.

Esto representa otro motivo por el cual no es suficiente conectar simplemente un iPhone al equipo Windows y copiar la aplicación.

Los dispositivos Apple utilizan mecanismos de seguridad que verifican que las aplicaciones hayan sido correctamente firmadas y autorizadas para ejecutarse.

Por lo tanto, para que ASISGRU pueda pasar del entorno de desarrollo actual a un iPhone físico, sería necesario realizar una configuración adicional.

También se debe tener en cuenta la versión de iOS compatible con la aplicación. Las aplicaciones .NET MAUI que utilizan Blazor tienen requisitos específicos de plataforma. La documentación actual de Microsoft establece, para la versión correspondiente de .NET MAUI, un requisito mínimo de iOS 16.4 para aplicaciones .NET MAUI Blazor.

Esto significa que, además del proceso de compilación, es necesario verificar que el dispositivo donde se pretende ejecutar la aplicación sea compatible con los requisitos de la versión de .NET MAUI utilizada.

---

# 7. ¿Significa esto que ASISGRU no puede utilizarse en iPhone?

No.

Es importante aclarar que la aplicación **no está limitada permanentemente a Android**.

ASISGRU fue desarrollada utilizando .NET MAUI, una tecnología cuyo propósito es facilitar la creación de aplicaciones para diferentes plataformas a partir de un proyecto común.

La dificultad actual consiste en que el proceso de desarrollo se realizó principalmente desde Windows y no se dispone del equipo Mac necesario para completar la compilación nativa para iOS.

Por lo tanto, existen dos situaciones diferentes.

### Situación actual

La aplicación puede continuar desarrollándose desde Windows y puede probarse en Android utilizando las herramientas disponibles.

### Situación necesaria para iOS

Para generar y probar correctamente una versión destinada a iPhone es necesario incorporar al proceso un equipo Mac compatible con las herramientas de Apple.

Esto significa que el proyecto realizado hasta ahora sigue siendo útil. No sería necesario volver a programar desde cero la aplicación solamente por querer agregar soporte para iOS.

La documentación de Microsoft confirma que Visual Studio en Windows puede trabajar con un Mac como host de compilación mediante Pair to Mac.

De esta forma, el código desarrollado para ASISGRU puede seguir siendo la base del proyecto y posteriormente configurarse y probarse para iOS.

---

# 8. Alternativas para continuar el proyecto

La ausencia de un equipo Mac propio no significa necesariamente que el proyecto tenga que detenerse.

Una primera alternativa consiste en continuar todo el desarrollo desde Windows y dejar la preparación de iOS para una etapa posterior. De esta forma se puede terminar el funcionamiento de ASISGRU, realizar las pruebas correspondientes en Android y corregir cualquier problema antes de trabajar con iOS.

Una segunda alternativa consiste en utilizar temporalmente un Mac disponible y configurarlo como equipo de compilación. Microsoft permite que Visual Studio se conecte a un Mac mediante la función Pair to Mac. Para ello, el Mac debe ser accesible mediante la red y tener configurado el acceso remoto.

Una tercera posibilidad es trabajar con un entorno donde se tenga acceso remoto a un Mac. En este caso, la parte de desarrollo puede continuar realizándose desde Windows, mientras que el equipo Mac se utiliza cuando sea necesario realizar tareas específicas de compilación para iOS.

Lo importante es comprender que el requisito no consiste necesariamente en comprar un Mac para escribir cada línea de código. El requisito fundamental es **tener acceso a un entorno Mac cuando se necesiten las herramientas de compilación de Apple**.

---

# 9. Conclusión

Después de analizar el proceso de desarrollo de ASISGRU y los requisitos de .NET MAUI para iOS, se puede concluir que la principal razón por la cual la aplicación no puede utilizarse actualmente en un iPhone no es un problema relacionado directamente con el código desarrollado.

El inconveniente se encuentra principalmente en el entorno de desarrollo utilizado y en los requisitos específicos de Apple para la creación de aplicaciones iOS.

ASISGRU fue desarrollada utilizando C#, .NET 10, .NET MAUI, Blazor, Visual Studio y SQLite. Estas tecnologías permiten desarrollar aplicaciones multiplataforma y, por lo tanto, el proyecto puede tener como objetivo tanto Android como iOS. Sin embargo, para generar una aplicación iOS es necesario utilizar las herramientas de compilación de Apple.

Estas herramientas se encuentran disponibles en macOS mediante Xcode. Microsoft establece que la compilación de aplicaciones nativas iOS con .NET MAUI requiere acceso a estas herramientas y, por ello, cuando el desarrollo se realiza desde Windows, Visual Studio debe conectarse a un Mac que funcione como equipo de compilación.

Por esta razón, desde el equipo Windows utilizado para desarrollar ASISGRU se puede continuar trabajando en el código, realizar modificaciones y desarrollar nuevas funciones, pero no es posible completar de manera independiente todo el proceso necesario para crear la versión nativa de iOS.

Para conseguir que ASISGRU pueda ejecutarse en un iPhone sería necesario incorporar un Mac compatible con Xcode al proceso de desarrollo, configurar la conexión con Visual Studio y realizar posteriormente los procesos de compilación, firma, pruebas y distribución correspondientes.

También sería necesario considerar los requisitos de Apple relacionados con el Apple ID, el programa de desarrolladores y la configuración del dispositivo cuando se pretenda realizar una implementación física o publicar la aplicación.

En conclusión, **ASISGRU no puede utilizarse actualmente en un iPhone desde el mismo entorno Windows en el que fue desarrollada porque el proceso de compilación para iOS depende de herramientas de Apple que requieren macOS**.
