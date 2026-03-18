# 📦 Práctica Git - Control de versiones

## 📌 Descripción del proyecto

Este repositorio contiene una práctica enfocada en el uso de Git como sistema de control de versiones. El objetivo principal es aprender a gestionar cambios, trabajar con ramas y mantener un historial de commits claro y profesional.

## 🛠️ Tecnologías utilizadas

* Git
* GitHub

## 🌿 Flujo de trabajo con ramas

Para el desarrollo del proyecto se ha seguido un flujo basado en ramas (branching):

* `main`: rama principal que contiene la versión estable del proyecto.
* `feature/login`: rama utilizada para desarrollar una funcionalidad específica (login).
* `feature/ui`: rama destinada a la mejora de la interfaz.

Cada funcionalidad se ha desarrollado de forma aislada en su propia rama, lo que permite trabajar de forma organizada sin afectar directamente a la rama principal.

Una vez finalizadas las funcionalidades, se ha realizado un **merge hacia la rama main**, integrando los cambios de forma controlada.

Este enfoque sigue buenas prácticas similares a metodologías como Git Flow simplificado.

## 🔀 Gestión de commits

Se han utilizado commits semánticos para mantener un historial claro:

* `feat:` → nuevas funcionalidades
* `fix:` → corrección de errores
* `docs:` → cambios en documentación
* `refactor:` → mejoras internas sin cambiar funcionalidad

Esto facilita la lectura del historial y mejora el trabajo en equipo.

## 🚫 Archivo .gitignore

Se ha configurado un archivo `.gitignore` para evitar subir archivos innecesarios al repositorio, como dependencias, logs o archivos compilados.

## ✅ Conclusión

Esta práctica demuestra el uso profesional de Git, aplicando buenas prácticas como el uso de ramas, commits semánticos, control de versiones y documentación adecuada del proyecto.
