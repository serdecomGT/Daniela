# MAC

1. Preparar una Mac

Primero se necesita tener acceso a una computadora Mac. En ella se debe instalar Xcode, que es la herramienta de Apple necesaria para desarrollar y compilar aplicaciones para iPhone.

Después de instalar Xcode, es importante abrirlo por primera vez para que termine de instalar los componentes necesarios.

También se debe verificar que la versión de Xcode sea compatible con la versión de .NET que se está utilizando en AsisGru.

2. Preparar la conexión entre Windows y la Mac

Como el proyecto actualmente se encuentra en Windows, Visual Studio puede conectarse a la Mac para utilizar las herramientas de Apple.

En la Mac se debe activar el Inicio de sesión remoto, que se encuentra en:

Configuración del sistema → General → Compartir → Inicio de sesión remoto

Esto permite que Visual Studio pueda comunicarse con la Mac.

Lo recomendable es que ambas computadoras estén conectadas a la misma red para facilitar la conexión.

3. Conectar Visual Studio con la Mac

Después de preparar la Mac, se abre el proyecto de AsisGru en Visual Studio 2026 desde Windows.

En Visual Studio se busca la opción para conectar la Mac, normalmente ubicada en:

Tools → iOS → Pair to Mac

o, dependiendo del idioma:

Herramientas → iOS → Conectar a Mac

Se selecciona la Mac y se realiza la conexión utilizando el usuario y las credenciales correspondientes.

Una vez conectadas, Visual Studio podrá utilizar la Mac para realizar la compilación de la aplicación para iOS.

4. Comprobar que esté disponible iOS

Después de conectar correctamente la Mac, Visual Studio debería permitir seleccionar un destino para iOS.

Por ejemplo:

Android Emulator
Windows Machine
iOS Simulator
iOS Remote Device

Antes de intentar instalar la aplicación en un iPhone real, es recomendable utilizar primero un simulador de iOS.

Esto permite comprobar que AsisGru funciona correctamente en el sistema de Apple.

5. Probar AsisGru en iOS

Al ejecutar AsisGru mediante el simulador, se debe comprobar que las diferentes partes de la aplicación continúen funcionando correctamente.

Por ejemplo:

Pantallas de la aplicación.
Botones y formularios.
Navegación entre páginas.
Registro de participantes.
Registro de categorías.
Registro de actividades.
Registro de asistencia.
Base de datos SQLite.
Página de créditos.
Logotipo e imágenes.
Funcionamiento sin conexión a Internet.

Esto es importante porque, aunque la aplicación sea la misma, es necesario comprobar que la interfaz y las funciones se comporten correctamente en iOS.

6. Probarla en un iPhone real

Cuando la aplicación funcione correctamente en el simulador, se puede pasar a realizar una prueba en un iPhone.

Para esto se conecta el dispositivo y se configura el proceso de desarrollo y aprovisionamiento de Apple.

En Visual Studio se podrá seleccionar el dispositivo iPhone como destino y ejecutar la aplicación.

De esta manera, la aplicación se compila utilizando la Mac y posteriormente se instala para realizar las pruebas directamente en el teléfono.

7. Configurar la cuenta de Apple

Para ejecutar y distribuir una aplicación de iOS también es necesario configurar los elementos de desarrollo de Apple.

Entre ellos se encuentran:

Apple ID.
Identificador de la aplicación.
Certificado de desarrollo.
Perfil de aprovisionamiento.

Por ejemplo, se puede utilizar un identificador como:

com.asisgru.app

Este identificador sirve para distinguir la aplicación dentro del sistema de Apple.

8. Generar la versión para iPhone

Cuando AsisGru ya haya sido probada y configurada correctamente, se puede generar la versión de distribución para iOS.

El resultado puede ser un archivo con extensión:

AsisGru.ipa

Este archivo corresponde al paquete de la aplicación para iOS y puede utilizarse dentro del proceso de distribución correspondiente de Apple.

En resumen

No es necesario volver a programar AsisGru desde cero para hacerla funcionar en iPhone. La aplicación ya fue desarrollada con .NET MAUI / Blazor, por lo que se puede trabajar sobre el mismo proyecto.

Lo que cambia principalmente es el proceso de compilación: Android se puede desarrollar y compilar desde Windows, mientras que para iOS se necesita una Mac con Xcode.

Por lo tanto, el proceso sería:

AsisGru actual
      ↓
Proyecto .NET MAUI
      ↓
Visual Studio en Windows
      ↓
Conexión con una Mac
      ↓
Xcode
      ↓
Compilación para iOS
      ↓
Pruebas en iPhone
      ↓
Versión final de AsisGru para iOS

Y no se tendría que modificar toda la aplicación, sino revisar que el proyecto actual esté correctamente preparado para incluir el destino de iOS y posteriormente realizar las configuraciones propias de Apple.
   
