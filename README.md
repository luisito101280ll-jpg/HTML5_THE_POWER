# HTML5 The Power

Repositorio de prácticas del curso de HTML5. Cada carpeta corresponde a un bloque temático con sus ejercicios y proyectos.

🌐 **Demo en vivo:** [html5-the-power.netlify.app](https://html5-the-power.netlify.app)

---

## Temario practicado

### 01 · Estructura básica de HTML5
**Carpeta:** `01-estructura/`

Primera página funcional. Conceptos aplicados:
- Declaración `<!DOCTYPE html>` y atributo `lang`
- Secciones obligatorias: `<head>` y `<body>`
- Metaetiquetas esenciales: `charset` y `viewport`
- `<title>` para el nombre de la pestaña
- Etiquetas de bloque básicas: `<h1>` y `<p>`

---

### 02 · Texto, Listas y Enlaces
**Carpeta:** `02-texto-listas-enlaces/`

Tres archivos: página principal, página de prácticas y ejercicio de calentamiento. Conceptos aplicados:
- Listas no ordenadas `<ul>` y ordenadas `<ol>` con `<li>`
- Sublistas: un `<li>` que contiene otro `<ul>` o `<ol>`
- Barra de navegación con `<nav>` y `<a href>`
- Enlaces a otras páginas del mismo proyecto (rutas relativas)
- Enlaces externos con `target="_blank"`
- Anclas internas: atributo `id` + `href="#id"`
- Enlace de retorno a la parte superior de la página

---

### 03 · Imágenes, Media, Interactividad y DOM
**Carpeta:** `03-imagenes-media/`

Clon simplificado de YouTube. El ejercicio más completo hasta ahora — combina estructura semántica con elementos interactivos y una introducción a JavaScript en el navegador. Conceptos aplicados:

**Elementos interactivos nativos**
- `<details>` + `<summary>` — sección colapsable sin necesidad de JavaScript
- `<dialog>` con `showModal()` y `close()` — modales nativos del navegador
- Atributo `contenteditable` — hace cualquier elemento editable en el navegador
- `placeholder` en `<input>` — texto de ayuda dentro del campo

**Tablas**
- `<table>`, `<tr>`, `<th>`, `<td>` — estructura básica de tabla de datos
- `<template>` — fragmento HTML reutilizable que no se renderiza hasta que JS lo inserta

**Scripts y módulos**
- `<script>` inline, externo (`src`) y como módulo ES6 (`type="module"` + `import`)
- `<script nomodule>` — fallback para navegadores sin soporte de módulos

**Eventos del DOM**
- Eventos como atributo HTML: `onclick`, `onblur`, `onfocus`
- `addEventListener("scroll", función)` — forma recomendada de escuchar eventos desde JS
- `document.getElementById()` — seleccionar elementos del DOM
- `element.innerHTML` — leer o modificar el contenido de un elemento
- `element.style.color` — modificar estilos desde JavaScript

**Lecciones clave del ejercicio**
- Los `id` deben ser únicos en toda la página; si se repiten, el JS solo encuentra el primero
- Separar funciones con nombres distintos evita que una sobreescriba a otra
- Las rutas a archivos deben ser relativas al proyecto, nunca rutas absolutas locales (`C:\Users\...`)

---

### 05 · Proyecto — Linktree personal
**Carpeta:** `05-linktree/`

Página de perfil con enlaces a redes sociales, al estilo Linktree. Conceptos aplicados:
- Etiquetas semánticas de estructura: `<header>`, `<main>`, `<section>`
- Imagen de perfil con `<img>` y atributo `alt`
- Lista de enlaces a perfiles externos (LinkedIn, web propia)

---

### 06 · Página de Noticias
**Carpeta:** `06-news/`

Dos archivos: portada de noticias y página de artículos. Conceptos aplicados:
- Semántica avanzada: `<article>`, `<aside>`, `<figure>`, `<figcaption>`
- Imágenes adaptables con `<picture>` y `<source media="...">`
- Atributo `srcset` para distintas resoluciones de pantalla
- Columna lateral con `<aside>` y lista de enlaces relacionados

---

### 07 · Landing page con formulario
**Carpeta:** `07-landing_form/`

Página de producto con secciones de características, testimonios, precios y contacto. Conceptos aplicados:
- Formulario completo con `<form>`, `<label>`, `<input>` y `<textarea>`
- Tipos de input: `text`, `email`, `submit`
- Asociación de etiquetas con campos mediante atributo `for` / `id`
- Estructura de landing: `<header>`, varias `<section>` temáticas y `<footer>`

---

### 08 · Portfolio personal
**Carpeta:** `08-portfolio/`

Dos versiones de portfolio personal. Conceptos aplicados:
- Página de presentación profesional completa
- Navegación interna mediante `<nav>` con anclas a cada sección
- Enlace de correo electrónico con protocolo `mailto:`
- Texto con énfasis usando `<strong>`
- `<footer>` con copyright usando la entidad `&copy;`
- Versión alternativa con `<article>` para proyectos individuales

---

## Chuleta de referencia
**Carpeta:** `docs_chuleta/`

Documento de consulta rápida y diario de aprendizaje en formato Markdown. Incluye todas las etiquetas practicadas, ejemplos mínimos funcionales y un sistema de repaso espaciado.

---

### 10 · Iniciación a CSS
**Carpeta:** `10 - css/01-iniciacion/`

Primera página con estilos reales. Conceptos aplicados:
- Vincular hoja de estilos externa: `<link rel="stylesheet" href="style.css">`
- Selectores de elemento: `body`, `header`, `main`, `article`, `h1`, `p`, `a`, `li`
- Colores: `color`, `background-color`, valores hexadecimales (`#111`, `#eee`) y nombres (`crimson`, `grey`)
- Tipografía: `font-family`, `font-size`, `font-weight`, `font-style`, `text-transform`, `text-align`, `line-height`
- Espaciado y bordes: `margin`, `padding`, `border`, `border-radius`
- Centrado de bloque: `max-width` + `margin: 0 auto`
- Stack de fuentes del sistema: `system-ui, Arial, sans-serif`

---

## Estado del temario

| Bloque | Tema | Estado |
|--------|------|--------|
| 01 | Estructura básica | Completado |
| 02 | Texto, listas y enlaces | Completado |
| 03 | Imágenes, media, interactividad y DOM | Completado |
| 04 | Formularios | Pendiente |
| 05 | Proyecto Linktree | Completado |
| 06 | Página de noticias | Completado |
| 07 | Landing con formulario | Completado |
| 08 | Portfolio personal | Completado |
| 10 | Iniciación a CSS | En curso |

---

*Autor: Luis Angel Lozano Gascón — Futuro Developer Full Stack*
