# HTML — Chuleta + Diario (RTC)

<aside>

**Cómo usar esto (2 min/día)**
1) Actualiza solo la *Chuleta (1 línea)*
2) Haz *1 mini-ejercicio*
3) Si algo falla, anota *1 duda*

</aside>

---

## Chuleta

### Estructura base
- Esqueleto: `<!DOCTYPE html>` → `<html lang="es">` → `<head>` → `<body>`
- Meta obligatorias: `<meta charset="UTF-8">` + `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
- Pestaña del navegador: `<title>...</title>` (dentro de `<head>`)
- Bloques de texto: `<h1>`–`<h6>` (títulos), `<p>` (párrafo)

### Listas y enlaces
- Listas: `<ul>` (sin orden), `<ol>` (con orden), `<li>` (elemento)
- Sublistas: un `<li>` puede contener otro `<ul>` u `<ol>`
- Enlace externo: `<a href="https://..." target="_blank">texto</a>`
- Enlace a otra página: `<a href="./pagina.html">texto</a>`
- Enlace interno (ancla): `<a href="#id">texto</a>` + `id="id"` en el destino
- Enlace de email: `<a href="mailto:correo@mail.com">texto</a>`

### Semántica estructural
- Cabecera de página o sección: `<header>`
- Navegación principal: `<nav>`
- Contenido principal: `<main>`
- Sección temática: `<section>`
- Contenido independiente (noticia, post): `<article>`
- Contenido relacionado secundario: `<aside>`
- Pie de página: `<footer>`

### Imágenes y media
- Imagen básica: `<img src="ruta.jpg" alt="descripción">`  → `alt` es obligatorio para accesibilidad
- Imagen con pie: `<figure>` + `<img>` + `<figcaption>descripción</figcaption>` + `</figure>`
- Imagen responsive (varias resoluciones):
```html
<picture>
  <source media="(min-width: 768px)" srcset="imagen-grande.jpg">
  <source media="(min-width: 480px)" srcset="imagen-media.jpg">
  <img src="imagen-pequeña.jpg" alt="descripción">
</picture>
```

### Formularios
- Contenedor: `<form>`
- Campo de texto: `<input type="text" id="nombre" name="nombre">`
- Campo de email: `<input type="email" id="email" name="email">`
- Área de texto: `<textarea id="mensaje" name="mensaje" rows="5"></textarea>`
- Botón de envío: `<input type="submit" value="Enviar">`
- Etiqueta asociada: `<label for="nombre">Nombre:</label>` → `for` debe coincidir con el `id` del input

### Texto y entidades
- Negrita semántica: `<strong>texto importante</strong>`
- Copyright: `&copy;` → se renderiza como ©
- Salto de línea: `<br>`

---

## Diario (una entrada por día)

### 2026-05-19 — Estructura, listas y enlaces

**3 ideas**

- `head` vs `body`
- `<title>` cambia la pestaña
- Listas (`ul/ol/li`) + sublistas + enlaces (`a`)

**1 ejemplo mínimo**

```html
<a href="#pasos">Ir a pasos</a>
<h2 id="pasos">Pasos</h2>
```

**1 mini-ejercicio (hecho)**

- Crear `index.html` + listas + sublista + enlace interno + enlace externo
- Crear `practicas.html` y navegar ida/vuelta

**1 duda (si aparece)**

- (vacío)

---

### 2026-05-20 — Semántica estructural · Proyecto Linktree

**3 ideas**

- HTML semántico: las etiquetas describen el *significado* del contenido, no solo su aspecto
- `<header>`, `<main>`, `<section>` organizan la página en zonas con sentido
- `<img>` siempre necesita `alt` (accesibilidad + SEO)

**1 ejemplo mínimo**

```html
<header>
  <img src="perfil.jpg" alt="Foto de perfil">
  <h1>Luis Angel Lozano</h1>
</header>
<main>
  <section>
    <ul>
      <li><a href="https://linkedin.com/in/...">LinkedIn</a></li>
    </ul>
  </section>
</main>
```

**1 mini-ejercicio (hecho)**

- Construir una página estilo Linktree con `<header>`, `<main>`, `<section>` y lista de enlaces externos

**1 duda (si aparece)**

- (vacío)

---

### 2026-05-21 — Imágenes responsive · Página de noticias

**3 ideas**

- `<article>` agrupa contenido que tiene sentido por sí solo (una noticia, un post)
- `<aside>` es contenido relacionado pero secundario (sidebar, noticias relacionadas)
- `<picture>` + `<source media>` sirve para cargar imágenes distintas según el tamaño de pantalla

**1 ejemplo mínimo**

```html
<figure>
  <picture>
    <source media="(min-width: 768px)" srcset="grande.jpg">
    <img src="pequeña.jpg" alt="Descripción">
  </picture>
  <figcaption>Pie de foto</figcaption>
</figure>
```

**1 mini-ejercicio (hecho)**

- Maquetar una portada de noticias con `<article>`, `<section>`, `<aside>`, `<figure>` y `<picture>`

**1 duda (si aparece)**

- (vacío)

---

### 2026-05-21 — Formularios · Landing page

**3 ideas**

- `<label for="id">` debe coincidir con el `id` del `<input>` al que describe
- Cada campo tiene un `type` que cambia su comportamiento: `text`, `email`, `submit`
- `<textarea>` es para textos largos; `<input>` para textos cortos de una línea

**1 ejemplo mínimo**

```html
<form>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email">
  <textarea id="mensaje" name="mensaje" rows="5"></textarea>
  <input type="submit" value="Enviar">
</form>
```

**1 mini-ejercicio (hecho)**

- Construir una landing page completa con `<header>`, secciones de producto, testimonios, precios y formulario de contacto en `<footer>`

**1 duda (si aparece)**

- (vacío)

---

### 2026-05-21 — Portfolio personal completo

**3 ideas**

- `<nav>` dentro del `<header>` con anclas internas conecta el menú con cada sección
- `mailto:` en un `<a href>` abre el cliente de correo del usuario directamente
- `&copy;` es una entidad HTML que evita problemas de codificación al escribir ©

**1 ejemplo mínimo**

```html
<nav>
  <ul>
    <li><a href="#proyectos">Proyectos</a></li>
    <li><a href="#contacto">Contacto</a></li>
  </ul>
</nav>
...
<footer>
  <p>&copy; 2026 Luis Angel Lozano</p>
  <a href="mailto:correo@mail.com">Escríbeme</a>
</footer>
```

**1 mini-ejercicio (hecho)**

- Construir dos versiones de portfolio: una con lista de proyectos y otra con `<article>` por proyecto, comparando ambas estructuras

**1 duda (si aparece)**

- (vacío)

---

## Repaso espaciado (para no olvidar)

- **Día 1 tras cada bloque:** reescribe la estructura sin mirar (5 min)
- **Día 3:** escribe un formulario con `<label>` + `<input>` + `<textarea>` de memoria
- **Día 7:** maqueta una página con semántica completa: `<header>`, `<nav>`, `<main>`, `<article>`, `<aside>`, `<footer>`
- **Día 14:** construye un Linktree y una página de noticias con imagen responsive desde cero
