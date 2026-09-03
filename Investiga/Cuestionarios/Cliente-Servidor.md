# Cuestionario: Arquitectura Cliente-Servidor

**Nombre del entrevistado:** Daniela Alejandra López de León
**Fecha:** 3 de septiembre 
**Nivel de experiencia:** Principiante

---

## Sección A — Conceptos fundamentales

1. ¿Qué es la arquitectura cliente-servidor? Explica con tus propias palabras.
Es un modelo donde el cliente solicita información y el servidor la proporciona.

2. ¿Qué es un **cliente** en esta arquitectura? Da un ejemplo cotidiano.
Es el dispositivo o programa que solicita un servicio. Ejemplo: ***Google Chrome***.

3. ¿Qué es un **servidor** en esta arquitectura? Da un ejemplo cotidiano.
Es el sistema que recibe solicitudes y proporciona información o servicios.

4. ¿Cuál es la diferencia entre un cliente y un servidor?
El cliente solicita y el servidor responde.

5. Dibuja o describe con palabras el flujo de comunicación entre un cliente y un servidor cuando visitas una página web.
***Cliente = Solicitud = Servidor = Respuesta = Página web***.

## Sección B — Protocolos y comunicación

6. ¿Qué es el protocolo HTTP y qué función cumple en la arquitectura cliente-servidor?
Es un protocolo que permite la comunicación entre clientes y servidores.

7. ¿Cuál es la diferencia entre HTTP y HTTPS?
**HTTPS** cifra y protege la información; **HTTP no**.

8. ¿Qué son los métodos HTTP `GET`, `POST`, `PUT` y `DELETE`? Explica cuándo se usa cada uno.
GET consulta, POST envía, PUT actualiza y DELETE elimina datos.

9. ¿Qué es una API REST y cómo se relaciona con la arquitectura cliente-servidor?
Es un servicio que permite que diferentes aplicaciones se comuniquen mediante **HTTP**.

10. ¿Qué es un código de estado HTTP? Menciona el significado de los códigos `200`, `404` y `500`.
***200 = correcto.***
***404 = no encontrado.***
***500 = error del servidor.***

## Sección C — Componentes y tipos

11. ¿Qué es un puerto de red y por qué es importante en la comunicación cliente-servidor? Menciona los puertos más comunes para HTTP y HTTPS.
Es un número que identifica un servicio de red. HTTP usa el 80 y HTTPS el 443.

12. ¿Cuál es la diferencia entre una arquitectura de **dos capas** y **tres capas** (3-tier)?
Dos capas separan cliente y servidor; tres capas separan presentación, lógica y datos.

13. ¿Qué es la capa de presentación, la capa lógica (de negocio) y la capa de datos?
**Presentación = interfaz.**
**Lógica = procesos.**
**Datos = almacenamiento.**

14. ¿Qué es un *proxy* y en qué situaciones se utiliza?
Es un intermediario entre el cliente y el servidor.

15. ¿Qué diferencia hay entre un servidor web y un servidor de aplicaciones?
El servidor web entrega contenido; el de aplicaciones ejecuta la lógica de la aplicación.

## Sección D — Contexto práctico

16. Cuando escribes una aplicación Blazor, ¿qué actúa como cliente y qué actúa como servidor?
Depende del tipo de Blazor. En **WebAssembly**, el navegador es el cliente; en **Blazor Server**, la aplicación funciona principalmente en el servidor.

17. ¿Qué es el *hosting* y cómo se relaciona con los servidores?
Es un servicio que permite almacenar y publicar una aplicación o página web.

18. ¿Qué es la latencia de red y cómo afecta la experiencia del usuario?
Es el tiempo que tarda la información en viajar por la red. Una latencia alta hace más lenta la aplicación.

19. ¿Qué es un *endpoint*? Da un ejemplo.
Es una dirección específica de una API para acceder a un recurso. Ejemplo: **/api/usuarios**.

20. ¿Qué es la escalabilidad y por qué es importante en un servidor?
Es la capacidad de un sistema para soportar más usuarios o trabajo sin perder rendimiento.

## Sección E — Pregunta reflexiva

21. ¿Por qué crees que la arquitectura cliente-servidor es el modelo más utilizado en Internet actualmente? ¿Conoces alguna alternativa?
Porque permite compartir servicios y datos de forma organizada. Una alternativa es P2P, donde los dispositivos se comunican directamente entre sí.
