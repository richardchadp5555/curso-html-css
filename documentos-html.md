# 🌐 Documentos HTML

Recopilación de teoría básica sobre HTML basada en el curso introductorio. Esta documentación incluye aspectos clave como su evolución, estructura y elementos principales.

---

## 1️⃣ Evolución de HTML hasta HTML5

HTML (HyperText Markup Language) es el lenguaje base para la construcción de páginas web. A lo largo de los años, ha evolucionado para adaptarse a las necesidades del desarrollo moderno:

- **HTML 1.0 (1993):** La primera versión, limitada y muy básica.
- **HTML 4.01 (1999):** Amplió capacidades con el uso de tablas, formularios y estilos básicos.
- **XHTML (2000):** Una versión más estricta y basada en XML.
- **HTML5 (2014):** Introdujo soporte para multimedia (audio, video) y elementos semánticos como `<header>`, `<article>`, y `<footer>`. Además, eliminó elementos obsoletos como `<font>`.

---

## 2️⃣ Etiquetas, Atributos y Comentarios

### 🏷️ **Etiquetas**
Las etiquetas son la base del HTML, utilizadas para estructurar el contenido. Cada etiqueta se compone de una apertura y un cierre, como:
```html
<h1>Esto es un encabezado</h1>
<p>Esto es un párrafo</p>
```

---

### ⚙️ **Atributos**
Los atributos proporcionan información adicional a las etiquetas y se definen dentro de la apertura. Ejemplo:
```html
<img src="imagen.jpg" alt="Descripción de la imagen">
```

---

### 💬 **Comentarios**
Los comentarios se utilizan para añadir notas en el código que no serán visibles para el usuario:
```html
<!-- Esto es un comentario -->
```

---

## 3️⃣ Estructura de una Página Web (Árbol DOM)

### 📂 **Estructura del DOM**
El DOM (Document Object Model) es una representación jerárquica de los elementos de una página web. La estructura típica es:
- `<html>`: Raíz del documento.
  - `<head>`: Contiene metadatos como título, enlaces a CSS o scripts.
  - `<body>`: Contiene el contenido visible de la página.

Ejemplo visual del DOM:

```
HTML
├── HEAD
│   ├── TITLE
│   ├── META
│   └── ...
└── BODY
    ├── HEADER
    ├── SECTION
    └── FOOTER
```

---

### 📖 **Cabecera de una Página Web**
La cabecera (`<head>`) incluye información que no se muestra directamente en la página, pero es esencial para su funcionamiento:
- `<title>`: Título que aparece en la pestaña del navegador.
- `<meta>`: Metadatos, como la codificación de caracteres.
  - Ejemplos comunes de meta etiquetas:
    ```html
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="description" content="Página web de ejemplo">
    <meta name="keywords" content="tienda, boniatos, sevilla">
    <meta name="author" content="Tu Nombre">
    ```
- `<link>`: Enlace a archivos CSS.
- `<script>`: Enlace a archivos JavaScript.

Ejemplo completo de `<head>`:
```html
<head>
    <title>Mi Primera Página</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="description" content="Página web de ejemplo">
    <meta name="keywords" content="tienda, boniatos, sevilla">
    <meta name="author" content="Tu Nombre">
    <link rel="stylesheet" href="styles.css">
    <script src="app.js"></script>
</head>
```

---

## 4️⃣ Añadiendo Contenido: Etiquetas Básicas

### 📰 **Encabezados**
Los encabezados estructuran el contenido en niveles jerárquicos, del más importante (`<h1>`) al menos importante (`<h6>`):
```html
<h1>Título Principal</h1>
<h2>Sección Importante</h2>
<h3>Subsección</h3>
<h4>Detalles</h4>
<h5>Menor Detalle</h5>
<h6>Nota Final</h6>
```

---

### 🖋️ **Etiquetas de Formato**
Estas etiquetas permiten cambiar el estilo del texto dentro de un documento:
- **Negrita:** `<b>Texto</b>`
- **Cursiva:** `<i>Texto</i>`
- **Tachado:** `<del>Texto</del>`
- **Énfasis:** `<em>Texto</em>`
- **Texto pequeño:** `<small>Texto</small>`
- **Superíndice:** `<sup>Texto</sup>`
- **Subíndice:** `<sub>Texto</sub>`

Ejemplo:
```html
<p>Este es un <b>texto en negrita</b>, y este es un <i>texto en cursiva</i>.</p>
```

---

### ✍️ **Otros Elementos**
- **Salto de línea:** `<br />`
- **Separador de temas:** `<hr />`
- **Párrafo:** `<p>Texto</p>`

Ejemplo:
```html
<p>Este es un párrafo.</p>
<hr />
<p>Otro párrafo tras un separador.</p>
```

---

