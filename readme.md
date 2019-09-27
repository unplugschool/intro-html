![](assets/img/logo.png)

---

# Introduction ⏳

-

## About you 🙋🏻‍♀️

- Name, likes, work
- What brought you to this workshop?
- What do you expect to get out of it?

-

## About me 🙋🏻‍♂️

- Web developer
- Tech & learning communities
- Unplug Studio & Unplug School
- Looking forward to help in your first steps

---

# Learning tips 📖

-

## Rules 📃

- There are no dumb questions
- Practice makes perfect
- Mistakes are part of the process
- You are in charge of learning

---

# What are we doing today? ⚡

-

## Today's project ☀

You'll create your own profile page on the internet. We won't be using social media nor other existing tools. You'll create your page from scratch, like a pro!

-

![Example profile page](assets/img/example.jpg)

-

### Get ready 😎

- Install a code editor
- Profile picture (Croppola)
- Favorite color code (W3 School: RGB Colors)
- Background image
- Favorite quote
- Likes and favorite link

-

### File structure 📂

- Create a file `index.html`
- Create a folder next to it `images`
- Put your images in the folder
- Let's avoid special characters and spaces in filenames

-

![Screenshot of file structure](assets/img/files.png)

---

# How does the Internet work? ☁

-

![Network map](assets/img/internet-nodes.png)

-

## Clients and servers

- Client: The device that requests the content
- Server: The device that serves the content

-

### 3 pillars of a website 🏠

- Hyper Text Markup Language (HTML): structure and meaning
- Cascading Style Sheets (CSS): appearance and layout
- JavaScript (JS): interactivity and advanced behavior

---

# HTML 👩🏻‍💻

Hyper Text Markup Language

-

HTML is not a programming language; it's a markup language. It's used to tell the browser how to display the sites you visit.

Notes:

This can be as complex or simple as the web designer desires it. HTML consists of a series of elements that wrap your content to look and behave as you want. With HTML you can make words link to other sites, add bold or italics, and more:

-

## HTML Elements

![Diagram of HTML element](assets/img/html-element.png)

Notes:

- Opening tag: consists of the name of the element (in this case "p"), enclosed by angle brackets. It establishes where the element starts to have its effect - in this case, where the paragraph starts.
- Closing tag: just like the opening tag, but includes a slash before the element name. Establishes where the element ends - in this case, where the paragraph ends.
- Content: the content of the element, in this case plain text.
- Element: the opening and closing tags, and the content enclosed by them.

-

## HTML Attributes

![HTML attribute diagram](assets/img/htmlatributos.png)

Notes:

Attributes contain additional (non-content) information about an element. In this case, the class attribute allows us to give the element a significative name that can be later used to style the element.

Attributes must always contain:

- A space separating it from the element name or other attributes.
- The name of the attribute, followed by the equal sign.
- Opening and closing tags enclosing the attribute's value

-

## Nested Elements

```html
<p>My cat is <strong>very</strong> grumpy.</p>
```

Notes:

You can also put elements inside another - this is called nesting. In this case we want to highlight a single word in the paragraph, so we enclose it in the `<strong>` element.

-

Order is important. *This is incorrect:*

```html
<p>My cat is<strong>very grumpy</p></strong>
```

Notes:

Elements must be openend and closed in an orderly manner, so that they are completely enclosed by other elements (no partial overlap). If elements overlap, the web browser will try to guess what you meant, and that can lead to unexpected and weird errors.

-

## HTML Skeleton

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My Profile</title>
  </head>
  <body>
    <img src="images/profile.png" alt="Photo of ...">
  </body>
</html>
```

Notes:

- `<!DOCTYPE html>` — the document type. There's a history on why you need it in your page, you don't need to know about it. Just put it in there.
- `<html></html>` — This is the top-level, all-enclosing element. Also known as the root element.
- `<head></head>` - Contains all non-visible content that is part of the page. Includes things like keywords, descriptions, references to CSS and JS, among others.
- `<body></body>` — Contains all content you want to display to your users including text, images, videos, games, audio tracks, and more.
- `<meta charset="utf-8">` — Important to make sure you can use non-ASCII characters in the content of your page.
- `<title></title>` — Establishes the page title that appears at the top of your window or tab. Also used by search engines.

-

## Images

```html
<img src="images/profile.jpg" alt="Photo of ...">
```

Use an `<img>` to add your photo.

Notes:

Como dijimos antes, incrusta una imagen en nuestra página, en la posición en que aparece. Lo logra a través del atributo src (source), el cual contiene el path (o ubicación) de nuestro archivo de imagen.

También incluimos un atributo alt (alternative) — el cual contiene un texto que debería describir la imagen, y que podría ser accedido por usuarios que no pueden ver la imagen

-

## Text

-

### Headings

```html
<h1>My main heading</h1>
<h2>My top level heading</h2>
<h3>My subtitle</h3>
<h4>My sub-subtitle</h4>
```

Add your name using `<h1>`.

Notes:

Los elementos de encabezado permiten especificar que ciertas partes del contenido son encabezados, o subencabezados del contenido. De la misma forma que un libro tiene un título principal, y que a su vez puede tener títulos por cada capítulo individual, y subtítulos dentro de ellos, un documento HTML puede tenerlos también. HTML posee seis niveles de encabezados, `<h1>–<h6>`, aunque probablemente sólo llegues a usar 3-4 como mucho:

-

### Paragraphs

```html
<p>This is just a paragraph</p>
```

Add your favorite quote inside a `<p>`.

-

### Numbered lists

`<ol>` stands for "ordered list" and `<li>` for "list item".

```html
<ol>
  <li>Crawl</li>
  <li>Walk</li>
  <li>Run</li>
</ol>
```

-

### Unordered lists

`<ul>` stands for "unordered list".

```html
<ul>
  <li>Dogs</li>
  <li>Cats</li>
  <li>Bunnies</li>
</ul>
```

Add an `<h2>` with the text "My favorites" and then add a `<ul>` with at least three `<li>` inside.

-

### Links

```html
<a>My favorite page</a>
```

Start with some text wrapped by `<a>`.

-

```html
<a href="">My favorite page</a>
```

Add the attribute: `href=""`.

-

```html
<a href="http://gooogle.com">Mi página favorita</a>
```

fill in the the `href` attribute with the URL.

-

## Result

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Profile - Ed Rivas</title>
</head>

<body>
    <img src="images/perfil.jpg" alt="Ed Rivas">
    <h1>Ed Rivas</h1>

    <p>Lorem ipsum dolor...</p>

    <h2>Favorites</h2>
    <ul>
        <li>HTML & CSS</li>
        <li>Video games</li>
        <li>Dogs y dinos</li>
        <li>Volunteering</li>
        <li>Twitter: <a href="http://twitter.com/je92rivas">@je92rivas</a></li>
    </ul>
</body>
</html>
```

-

![HTML-only page](assets/img/html-only.png)

Notes:

- Cambia el título de la pestaña modificando el `<title>`
- Observa como el navegador entiende que `<h1>` es más importante que `<h2>`.
- Observa que puedes hacer clic en el enlace y que el navegador te lleve a la página correcta

---

# CSS 🖌

Cascading Style Sheets

-

CSS is a *stylesheet language* which means it allows you to selectively style elements in your HTML document.

Notes:

Si HTML provee la estructura y el significado, CSS provee el estilo y diseño. Con CSS es posible controlar la apariencia de casi cualquier parte de una página web, incluyendo la tipografía, colores, disposición y tamaño de los elementos.

-

Create a file `style.css` next to `index.html`

```css
p {
    color: red;
}
```

-

Include your stylesheet in the `<head>` of your document.

```html
<head>
    <meta charset="UTF-8">
    <title>Profile - E Rivas</title>
    <link rel="stylesheet" href="style.css">
</head>
```

-

![HTML with paragraph styled red](assets/img/basic-css.png)

-

## CSS Rules

CSS stylesheets are a collection of rules

![Diagram of CSS rules](assets/img/csspartes.png)

Notes:

- **Selector**: El elemento HTML en el que comienza la regla. esta selecciona el(los) elemento(s) a dar estilo (en este caso, los elementos p ). Para dar estilo a un elemento diferente, solo cambia el selector.
- **Declaración**: Una sola regla como color: red; especifica a cuál de las propiedades del elemento quieres dar estilo.
- **Propiedades**: Maneras en las cuales puedes dar estilo a un elemento HTML. (En este caso, color es una propiedad del elemento p.) En CSS, seleccionas que propiedad quieres afectar en tu regla.
- **Valor de la propiedad**: A la derecha de la propiedad, después de los dos puntos (:), tenemos el valor de la propiedad, para elegir una de las muchas posibles apariencias para una propiedad determinada (hay muchos valores para color además de red).

-

Rules can include multiple declarations

```css
p {
    color: red;
    background-color: green;
}
```

Notes:

- Cada una de las reglas (aparte del selector) deben estar encapsulada entre corchetes ({}).
- Dentro de cada declaración, debes usar los dos puntos (:) para separar la propiedad de su valor.
- Dentro de cada regla, debes usar el punto y coma (;) para separar una declaración de la siguiente.

-

![Resultado de dos declaraciones CSS](assets/img/basic-css-2.png)

-

## Selectores

| Selector  | Selected element                     |
| --------  | ------------------------------------ |
| p, li, h1 | `<p>`, `<li>` y `<h1>`               |
| #my-id    | Element with `id="my-id"`            |
| .my-class | All elements with `class="my-class"` |

Notes:

- Selector de elemento: Todos los elementos HTML del tipo especificado
- Selector de identificación (ID): El elemento en la página con el ID especificado  (en una página HTML dada, solo se permite un unico elemento por ID).
- Selector de Clase: Los elementos en la página con la clase especificada (una clase puede aparecer varias veces en una página).

-

## Basic styles

```css
body {
    font-family: sans-serif;
    background-image: url(imagenes/fondo.jpg);
    background-size: cover;
    padding-top: 50px;
    padding-bottom: 50px;
}
```

Notes:

Aplica las declaraciones una por una y observa su efecto.

-

![Página con nuevo fondo aplicado](assets/img/css-1.png)

-

## Meet the `<div>`

Divs let us group elements to apply styles using CSS.

-

![Diseño por secciones](assets/img/example-annotated.jpg)

-

```html
<body>
    <div class="profile">
        <!-- Todo lo demás -->
    </div>
</body>
```

-

```html
<div class="header">
    <img src="images/profile.jpg" alt="...">
    <h1>Ed Rivas</h1>
</div>
```

-

```html
<div class="details">
    <p>Lorem ipsum...</p>
    <h2>Favorites</h2>
    <ul>...</ul>
</div>
```

-

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Profile - Ed Rivas</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <div class="profile">
    <div class="header">
      <img src="images/profile.jpg" alt="Ed Rivas">
      <h1>Ed Rivas</h1>
    </div>

    <div class="dtails">
      <p>Lorem ipsum...</p>
      <h2>Favorites</h2>
      <ul>
        <li>HTML & CSS</li>
        <li>Video games</li>
      </ul>
    </div>
  </div>

</body>
</html>
```

Notes:

Verifica que el `<body>` de tu documento se vea como lo que ves arriba. Lo importante es que tengas tres divs con las clases correctas aplicadas. El resultado en el navegador se verá idéntico, ya que las divs no producen ningún cambio hasta que se les aplican estilos.

-

Add a new rule to `style.css`, save the file and refresh your browser.

```css
.profile {
    background-color: #fff;
    margin-left: auto;
    margin-right: auto;
    width: 500px;
}
```

-

![](assets/img/css-2.png)

-

```css
.header {
    background-color: #00443A;
    padding-bottom: 10px;
    padding-top: 40px;
    text-align: center;
    color: #fff;
}
```

-

![](assets/img/css-3.png)

-

```css
.header img {
    border-color: #fff;
    border-radius: 100%;
    border-style: solid;
    border-width: 10px;
    max-width: 35%;
}
```

Notes:

Ahora estamos utilizando el selector de clase y elemento juntos para indicar que queremos seleccionar la `<img>` que está dentro de la div con clase "cabecera".

-

![](assets/img/css-4.png)

-

```css
.details {
    padding-top: 10px;
    padding-bottom: 10px;
    padding-left: 30px;
    padding-right: 30px;
}
```

-

![](assets/img/css-5.png)

-

```css
.details ul {
    padding-left: 20px;
}
```

-

![](assets/img/css-6.png)

Notes:

Prueba con estas propiedas:

- font-size: 50px
- font-style: italic
- line-height: 2
- text-shadow: 0 0 50px black
- box-shadow: 0 0 50px black

-

## 🎉 Well done! 🎉

You've created your first web page

Notes:

Si hay tiempo, compartir instrucciones para enviar y subir el trabajo realizado.

---

# Summary 🔃

-

## Internet ☁

- A network of computers
- Clients and servers
- Uses HTML, CSS, & JavaScript

-

## HTML 👩🏻‍💻

- Markup language
- Provides structure and content
- Built with tags
- Tags can be nested
- Tags can have attributes

-

```html
<div class="header">
    <img src="images/profile.jpg" alt="Ed Rivas">
    <h1>Ed Rivas</h1>
</div>
```

-

## CSS 🖌

- Stylesheet language
- Defines style and appearance
- Built with rules
- Rules have selectors and declarations

-

```css
.header img {
    border-color: #fff;
    border-radius: 100%;
    border-style: solid;
    border-width: 10px;
    max-width: 35%;
}
```

-

## Questions? 🤔

---

# Next steps 🚀

-

- Practice makes perfect
- You're in charge of your learning process
- Learn from more resources
