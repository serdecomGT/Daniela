# Cuestionario: Git — Control de Versiones

**Nombre del entrevistado:** Daniela Alejandra López de León 

**Fecha:** 3 de septiembre

**Nivel de experiencia:** Principiante

---

## Sección A — Conocimientos generales

1. ¿Qué es un sistema de control de versiones (VCS) y por qué es importante?
Es una herramienta que registra los cambios de un proyecto y permite recuperar versiones anteriores.

2. ¿Quién creó Git y en qué año?
Fue creado por **Linus Torvalds en 2005**.

3. ¿Cuál es la diferencia entre Git y GitHub?
**Git** controla las versiones y **GitHub** permite almacenar y compartir repositorios en línea.

4. ¿Qué es un repositorio (*repository*) en Git?
Es el lugar donde se guardan los archivos y el historial de cambios de un proyecto.

5. ¿Git es un sistema de control de versiones distribuido o centralizado? ¿Qué implica eso?
Es distribuido, porque cada usuario puede tener una copia completa del repositorio.

## Sección B — Comandos básicos

6. ¿Qué hace el comando `git init`?
Crea un **nuevo repositorio Git** en una carpeta.

7. ¿Qué hace el comando `git clone`? ¿Cuándo lo usarías?
Copia un repositorio existente para trabajar con él localmente.

8. Explica el flujo de trabajo básico: `git add` → `git commit` → `git push`. ¿Qué hace cada paso?
*git add:* prepara los cambios.
*git commit*: guarda los cambios.
*git push:* sube los cambios al repositorio remoto.

9. ¿Qué es el *staging area* (área de preparación)?
Es el espacio donde se seleccionan los cambios que se incluirán en el próximo commit.

10. ¿Cuál es la diferencia entre `git pull` y `git fetch`?
**git pull** descarga y aplica cambios. **git fetch** solo descarga la información.

11. ¿Qué hace el comando `git status` y por qué es útil?
Muestra el estado actual de los archivos y cambios del proyecto.

## Sección C — Ramas y colaboración

12. ¿Qué es una *branch* (rama) en Git y para qué se utiliza?
Es una línea de trabajo independiente que permite desarrollar funciones sin afectar la rama principal.

13. ¿Cómo se crea y cambia a una nueva rama? Escribe los comandos.
git branch nueva-rama
git checkout nueva-rama

También se conocen como:
git switch -c nueva-rama

14. ¿Qué es un *merge* (fusión) y cuándo se realiza?
Es el proceso de unir los cambios de una rama con otra.

15. ¿Qué es un *conflicto de fusión* y cómo se resuelve?
Ocurre cuando dos cambios entran en conflicto. Se debe revisar y elegir qué cambios conservar.

16. ¿Qué es un *pull request* (PR) en GitHub y cuál es su propósito?
Es una solicitud para revisar y unir cambios de una rama a otra en GitHub.

## Sección D — Conceptos intermedios

17. ¿Qué es un archivo `.gitignore` y para qué sirve? Menciona un ejemplo de archivo que deberías ignorar.
Es un archivo que indica qué **archivos Git debe ignorar**. Por ejemplo, archivos temporales.

18. ¿Qué es un *commit* y qué información debe contener un buen mensaje de commit?
Es un *registro de cambios* realizados en el proyecto. Su mensaje debe explicar brevemente qué se modificó.

19. ¿Qué es `git log` y qué información te muestra?
Muestra el historial de commits del proyecto.

20. ¿Qué es un *fork* en GitHub y cómo se diferencia de un *clone*?
Un fork crea una copia del repositorio en tu cuenta de GitHub. Un clon copia el repositorio en tu computadora.

## Sección E — Pregunta reflexiva

21. Imagina que trabajas en un proyecto con dos compañeros más. Describe brevemente cómo usarías Git y GitHub para colaborar sin perder el trabajo de nadie.
Cada compañero trabajaría en su propia rama, haría commits de sus cambios y los subiría a GitHub. Después, usarían Pull Requests para revisar y unir los cambios sin perder el trabajo de los demás.

