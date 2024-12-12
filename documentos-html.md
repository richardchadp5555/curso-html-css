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
- `<link>`: Enlace a archivos CSS.
- `<script>`: Enlace a archivos JavaScript.

Ejemplo:
```html
<head>
    <title>Mi Primera Página</title>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="styles.css">
    <script src="app.js"></script>
</head>
```

---

### Ejemplo Básico Completo:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Mi Primera Página</title>
    <meta charset="UTF-8">
</head>
<body>
    <h1>¡Hola Mundo!</h1>
    <p>Este es un ejemplo básico de HTML.</p>
</body>
</html>
```

---

Con esta información tienes una visión clara de los fundamentos de HTML. ¡Sigamos avanzando para profundizar más! 🚀

## Contacto
- ***autor**: Richard Chadwick PlaZA
- ***fecha**: 12/12/2024
