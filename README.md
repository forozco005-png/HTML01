# HTML01

# 🌐 Fundamentos de HTML

> Guía rápida para entender cómo se construye una página web desde cero. 🚀

---

## 📖 ¿Qué es HTML?

**HTML** (*HyperText Markup Language*) es el lenguaje que da **estructura** a las páginas web. 🧱

- 🏗️ No es un lenguaje de programación, es un lenguaje de **marcado**.
- 🏷️ Usa **etiquetas** para indicarle al navegador qué es cada contenido (título, párrafo, imagen, etc.).
- 🎨 Se combina con **CSS** (estilo) y **JavaScript** (interactividad).

| Tecnología | Función | Analogía 🏠 |
|------------|---------|-------------|
| HTML | Estructura | Los cimientos y las paredes |
| CSS | Diseño | La pintura y la decoración |
| JavaScript | Comportamiento | La electricidad y las puertas automáticas |

---

## 🧩 Estructura básica de un documento

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi primera página</title>
  </head>
  <body>
    <h1>¡Hola, mundo! 👋</h1>
    <p>Esta es mi primera página web.</p>
  </body>
</html>
```

### 🔍 ¿Qué hace cada parte?

- 📄 `<!DOCTYPE html>` → Indica que el documento usa HTML5.
- 🌍 `<html>` → Contenedor principal de toda la página. `lang="es"` define el idioma.
- 🧠 `<head>` → Información **invisible** para el usuario (título, codificación, estilos).
- 👀 `<body>` → Todo el contenido **visible** de la página.

---

## 🏷️ Anatomía de una etiqueta

```html
<p class="texto">Hola, soy un párrafo</p>
```

- 🔓 **Etiqueta de apertura:** `<p>`
- 🔒 **Etiqueta de cierre:** `</p>`
- ✍️ **Contenido:** `Hola, soy un párrafo`
- ⚙️ **Atributo:** `class="texto"` (da información extra al elemento)

> 💡 Algunas etiquetas no se cierran (*auto-cerradas*): `<br>`, `<img>`, `<hr>`, `<input>`.

---

## 📝 Etiquetas de texto

```html
<h1>Título principal</h1>
<h2>Subtítulo</h2>
<h3>Título de sección</h3>

<p>Un párrafo de texto.</p>
<strong>Texto importante</strong>
<em>Texto enfatizado</em>
<br>
<hr>
```

- 🔠 `<h1>` a `<h6>` → Encabezados (del más al menos importante).
- 📃 `<p>` → Párrafo.
- 💪 `<strong>` → Negritas (importancia).
- 🤏 `<em>` → Cursiva (énfasis).
- ↩️ `<br>` → Salto de línea.
- ➖ `<hr>` → Línea horizontal.

---

## 🔗 Enlaces e imágenes

### 🔗 Enlaces

```html
<a href="https://www.ejemplo.com" target="_blank">Visita el sitio</a>
```

- `href` → 📍 Dirección de destino.
- `target="_blank"` → 🪟 Abre el enlace en una pestaña nueva.

### 🖼️ Imágenes

```html
<img src="foto.jpg" alt="Descripción de la foto" width="300">
```

- `src` → 📂 Ruta de la imagen.
- `alt` → ♿ Texto alternativo (accesibilidad y por si la imagen no carga).

---

## 📋 Listas

### 🔢 Lista ordenada

```html
<ol>
  <li>Primer paso</li>
  <li>Segundo paso</li>
</ol>
```

### ⚫ Lista no ordenada

```html
<ul>
  <li>Manzana 🍎</li>
  <li>Plátano 🍌</li>
</ul>
```

---

## 📊 Tablas

```html
<table>
  <thead>
    <tr>
      <th>Nombre</th>
      <th>Edad</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Ana</td>
      <td>25</td>
    </tr>
  </tbody>
</table>
```

- 🗂️ `<table>` → Tabla.
- 🧾 `<tr>` → Fila.
- 🏷️ `<th>` → Celda de encabezado.
- 📦 `<td>` → Celda de datos.

---

## 📝 Formularios

```html
<form action="/enviar" method="post">
  <label for="nombre">Nombre:</label>
  <input type="text" id="nombre" name="nombre" placeholder="Tu nombre">

  <label for="correo">Correo:</label>
  <input type="email" id="correo" name="correo">

  <select name="pais">
    <option value="mx">México 🇲🇽</option>
    <option value="es">España 🇪🇸</option>
  </select>

  <textarea name="mensaje" rows="4"></textarea>

  <button type="submit">Enviar 📨</button>
</form>
```

Tipos de `<input>` comunes: `text`, `email`, `password`, `number`, `checkbox`, `radio`, `date`.

---

## 🏛️ Etiquetas semánticas

Dan **significado** al contenido y mejoran el SEO 🔎 y la accesibilidad ♿.

```html
<header>  Cabecera del sitio  </header>
<nav>     Menú de navegación   </nav>
<main>
  <section> Sección de contenido </section>
  <article> Artículo independiente </article>
  <aside>   Contenido lateral    </aside>
</main>
<footer>  Pie de página      </footer>
```

---

## 📦 `<div>` y `<span>`

- 📦 `<div>` → Contenedor de **bloque** (ocupa toda la línea).
- 🏷️ `<span>` → Contenedor **en línea** (solo ocupa lo necesario).

```html
<div class="tarjeta">
  <p>Texto con una <span class="resaltado">palabra destacada</span>.</p>
</div>
```

---

## 🆔 Atributos globales importantes

| Atributo | Uso | Emoji |
|----------|-----|-------|
| `id` | Identificador **único** de un elemento | 🆔 |
| `class` | Agrupa elementos con el mismo estilo | 🏷️ |
| `style` | Estilos en línea | 🎨 |
| `title` | Texto emergente al pasar el mouse | 💬 |
| `hidden` | Oculta el elemento | 🙈 |

---

## 💬 Comentarios

```html
<!-- Esto es un comentario, el navegador lo ignora 🙈 -->
```

---

## ✅ Buenas prácticas

1. 🔤 Escribe las etiquetas en **minúsculas**.
2. 🔒 **Cierra** siempre las etiquetas que lo requieran.
3. 🪆 **Indenta** el código para que sea legible.
4. ♿ Usa **`alt`** en todas las imágenes.
5. 🏛️ Prefiere etiquetas **semánticas** antes que `<div>` genéricos.
6. 🥇 Usa **un solo `<h1>`** por página.
7. ✔️ Valida tu código en el [Validador W3C](https://validator.w3.org/).

---

## 🛠️ ¿Cómo empezar a practicar?

1. 💻 Instala un editor de código como **VS Code**.
2. 📄 Crea un archivo llamado `index.html`.
3. ✍️ Copia la estructura básica de esta guía.
4. 🌐 Ábrelo con tu navegador (doble clic al archivo).
5. 🔄 Modifica, guarda y recarga para ver los cambios.

---

## 📚 Recursos para seguir aprendiendo

- 📘 [MDN Web Docs (Español)](https://developer.mozilla.org/es/docs/Web/HTML)
- 🎓 [W3Schools HTML](https://www.w3schools.com/html/)
- 🧪 [freeCodeCamp](https://www.freecodecamp.org/espanol/)

---

## 🎉 ¡Listo!

Ya conoces los fundamentos de HTML. El siguiente paso es aprender **CSS** para darle estilo a tus páginas. 🎨✨

> *"La práctica hace al maestro."* 💪
tos del html
[README_1.md](https://github.com/user-attachments/files/32858472/README_1.md)
