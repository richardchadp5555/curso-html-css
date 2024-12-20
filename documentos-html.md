# 🌐 Documentos HTML

Recopilación de teoría básica sobre HTML basada en el curso introductorio. Esta documentación incluye aspectos clave como su evolución, estructura y elementos principales.

---

## 1⃣ Evolución de HTML hasta HTML5

HTML (HyperText Markup Language) es el lenguaje base para la construcción de páginas web. A lo largo de los años, ha evolucionado para adaptarse a las necesidades del desarrollo moderno:

- **HTML 1.0 (1993):** La primera versión, limitada y muy básica.
- **HTML 4.01 (1999):** Amplió capacidades con el uso de tablas, formularios y estilos básicos.
- **XHTML (2000):** Una versión más estricta y basada en XML.
- **HTML5 (2014):** Introdujo soporte para multimedia (audio, video) y elementos semánticos como `<header>`, `<article>`, y `<footer>`. Además, eliminó elementos obsoletos como `<font>`.

---

## 2⃣ Etiquetas, Atributos y Comentarios

### 📜 **Etiquetas**
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

## 3⃣ Estructura de una Página Web (Arbol DOM)

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

## 4⃣ Añadiendo Contenido: Etiquetas Básicas

### 🌟 **Encabezados**
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

### 🔍 **Listas en HTML**
Las listas son muy utilizadas en HTML para organizar contenido:

#### 🔢 **Listas Numeradas (Ordenadas)**
Se crean con la etiqueta `<ol>` y cada elemento con `<li>`:
```html
<ol>
    <li>Primer elemento</li>
    <li>Segundo elemento</li>
    <li>Tercer elemento</li>
    <li>Cuarto elemento</li>
</ol>
```

#### 🔹 **Listas No Numeradas (Desordenadas)**
Se crean con `<ul>`:
```html
<ul>
    <li>Elemento 1</li>
    <li>Elemento 2</li>
    <li>Elemento 3</li>
</ul>
```

#### 📄 **Listas Anidadas**
Las listas pueden anidarse para crear subniveles:
```html
<ul>
    <li>Elemento 1
        <ul>
            <li>Subelemento 1.1</li>
            <li>Subelemento 1.2</li>
        </ul>
    </li>
    <li>Elemento 2</li>
</ul>
```

#### 🔗 **Listas de Definición**
Se utilizan para términos y sus descripciones con `<dl>`, `<dt>` y `<dd>`:
```html
<dl>
    <dt>HTML</dt>
    <dd>Lenguaje de la web</dd>
    <dt>CSS</dt>
    <dd>Hojas de estilo</dd>
</dl>
```

---

## 5⃣ Imágenes, Figuras y Rutas

### 🖼️ **Imágenes**
La etiqueta `<img>` se utiliza para insertar imágenes. Atributos frecuentes:
- **`src`:** Ubicación de la imagen.
- **`alt`:** Texto alternativo.
- **`width` y `height`:** Dimensiones.

Ejemplo:
```html
<img src="imagenes/ejemplo.jpg" alt="Descripción de la imagen" width="300" height="200">
```

### 🎮 **Figuras**
La etiqueta `<figure>` se utiliza para asociar imágenes con una descripción:
```html
<figure>
    <img src="img/openwebinars-logo.jpg" alt="Logo">
    <figcaption>Logotipo con la etiqueta figure</figcaption>
</figure>
```

### 🔍 **Rutas**
- **Relativa:** En relación al directorio del HTML.
- **Absoluta:** Ruta completa.
- **URL:** Dirección de Internet.

Ejemplo:
```html
<img src="imagenes/ejemplo.jpg" alt="Relativa">
<img src="https://ejemplo.com/imagen.jpg" alt="URL">
```

---

## 6⃣ Tablas en HTML

### 🔢 **Estructura Básica de una Tabla**
Una tabla básica se crea utilizando las etiquetas `<table>`, `<tr>`, `<th>`, y `<td>`.
- `<table>`: Define la tabla.
- `<tr>`: Define una fila.
- `<th>`: Define un encabezado de columna.
- `<td>`: Define una celda.

Ejemplo:
```html
<table>
    <tr>
        <th>Nombre</th>
        <th>Apellido</th>
    </tr>
    <tr>
        <td>Juan</td>
        <td>Pérez</td>
    </tr>
</table>
```

### 🌐 **Atributos Avanzados**
- **`rowspan`:** Permite que una celda ocupe más de una fila.
- **`colspan`:** Permite que una celda ocupe más de una columna.

Ejemplo:
```html
<table>
    <tr>
        <td rowspan="2">Matemáticas</td>
        <td>Lengua</td>
        <td colspan="2">Ciencias</td>
    </tr>
    <tr>
        <td>Historia</td>
        <td>Física</td>
        <td>Química</td>
    </tr>
</table>
```

### 💡 **Estilizando Tablas con CSS**
Podemos personalizar tablas utilizando CSS:

#### 📦 **Bordes Colapsados**
```css
table {
    border-collapse: collapse;
}
td, th {
    border: 1px solid black;
}
```

#### 🔹 **Bordes sin Colapsar**
```css
table, td, th {
    border: 1px solid black;
}
```

#### 🌍 **Bordes Específicos**
Podemos aplicar bordes específicos como "superior" o "inferior":
```css
td, th {
    border-bottom: 1px solid black;
}
```

---

Con esta información tienes una guía completa para trabajar con tablas en HTML. 🚀
