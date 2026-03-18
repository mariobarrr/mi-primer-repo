# 🌐 Mi Portfolio Web

Proyecto web personal desarrollado con HTML, CSS y JavaScript como práctica de flujo de trabajo Git profesional.

---

## 📋 Descripción

Portfolio web estático que muestra información personal, habilidades y proyectos. El objetivo principal de esta práctica es aplicar un flujo de trabajo Git estructurado con ramas, commits semánticos y resolución de conflictos.

---

## 🛠️ Tecnologías usadas

- HTML5
- CSS3 (con diseño responsive)
- JavaScript (vanilla)

---

## 🌿 Flujo de ramas usado

Este proyecto sigue un flujo de trabajo basado en **Feature Branching**:

```
main
├── feature/estructura-html   → estructura base del HTML
├── feature/estilos           → hoja de estilos CSS y responsive
└── feature/interactividad    → lógica JavaScript
```

### Proceso seguido

1. Se creó la rama `main` con los archivos iniciales (`README.md`, `.gitignore`)
2. Se abrió la rama `feature/estructura-html` para desarrollar el HTML base
3. Se abrió la rama `feature/estilos` para los estilos CSS
4. Se generó un **conflicto de merge intencional** entre `feature/estilos` y `feature/estructura-html` en el archivo `index.html`, modificando la misma línea en ambas ramas
5. El conflicto se resolvió manualmente editando el archivo y eligiendo la versión correcta
6. Finalmente, se hizo merge de todas las ramas a `main`

---

## ⚔️ Resolución de conflictos

Durante el merge de `feature/estilos` → `main` se produjo un conflicto en `index.html` porque ambas ramas habían modificado el título de la página (`<title>`).

Git marcó el conflicto así:

```
<<<<<<< HEAD
<title>Portfolio</title>
=======
<title>Mi Portfolio Personal</title>
>>>>>>> feature/estilos
```

Se resolvió manualmente eligiendo la versión más descriptiva: `<title>Mi Portfolio Personal</title>`, y luego se hizo `git add` y `git commit` para cerrar el merge.

---

## 🔀 Git merge vs Git rebase

| | `git merge` | `git rebase` |
|---|---|---|
| **Qué hace** | Une dos ramas creando un commit de merge | Reescribe los commits de una rama sobre otra |
| **Historial** | Conserva el historial completo con bifurcaciones | Produce un historial lineal y más limpio |
| **Cuándo usarlo** | En ramas compartidas o cuando quieres trazabilidad | En ramas locales antes de hacer merge para limpiar el historial |
| **Ejemplo** | `git merge feature/estilos` desde `main` | `git rebase main` desde `feature/estilos` |

En este proyecto se usó **merge** para conservar la trazabilidad de cada rama.

---

## 🚀 Cómo ejecutar el proyecto

```bash
# Clonar el repositorio
git clone <url-del-repo>

# Abrir el archivo principal
open index.html
# o simplemente arrástralo al navegador
```

---

## 📁 Estructura del proyecto

```
mi-portfolio/
├── index.html       # Página principal
├── style.css        # Estilos y diseño responsive
├── script.js        # Interactividad
├── .gitignore       # Archivos excluidos de Git
└── README.md        # Este archivo
```

---

*Desarrollado con ayuda de Claude (Anthropic) para los mensajes de commit y estructura del flujo Git.*