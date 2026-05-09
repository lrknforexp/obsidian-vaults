# HTML

> [!info] Quick Facts
> **Full Name:** HyperText Markup Language
> **Created:** 1991 by Tim Berners-Lee
> **Current Version:** HTML5 (2014, continuously updated)
> **Type:** Markup language (NOT a programming language)
> **Used For:** Structure and content of every web page on the internet
> **Difficulty:** ⭐ — The easiest thing to learn; start here
> **Official Reference:** https://developer.mozilla.org/en-US/docs/Web/HTML

---

**HTML** is the **skeleton of every web page**. It defines the structure and content — headings, paragraphs, images, links, buttons, forms, and everything else you see in a browser. Every website in existence uses HTML. It's not a programming language (it has no logic, no variables, no loops) — it's a **markup language** that tells the browser what things are.

---

## How HTML Works

An HTML file is just a text file ending in `.html`. Your browser reads it and renders it as a visual web page. HTML is made of **tags** — keywords wrapped in angle brackets:

```html
<tagname>Content goes here</tagname>
```

Most tags have an **opening tag** and a **closing tag** (with `/`):
```html
<h1>This is a heading</h1>
<p>This is a paragraph.</p>
```

Some tags are **self-closing** (no content inside):
```html
<img src="photo.jpg" alt="My photo" />
<br />
<input type="text" />
```

---

## The Basic HTML Document Structure

Every HTML file should start with this exact structure:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Page Title</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>

    <!-- Everything visible goes here -->
    <h1>Hello, World!</h1>
    <p>This is my web page.</p>

    <script src="script.js"></script>
  </body>
</html>
```

> [!info] What Each Part Does
> - `<!DOCTYPE html>` — tells the browser this is HTML5
> - `<html>` — the root element wrapping everything
> - `<head>` — invisible metadata (title, CSS links, settings)
> - `<title>` — the text shown in the browser tab
> - `<body>` — everything the user actually sees
> - `<!-- comment -->` — notes that the browser ignores

---

## Core HTML Tags

### Text
```html
<h1>Heading 1 (biggest)</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6 (smallest)</h6>

<p>This is a paragraph.</p>

<strong>Bold text</strong>
<em>Italic text</em>
<u>Underlined text</u>
<s>Strikethrough text</s>

<br />  <!-- line break -->
<hr />  <!-- horizontal rule (dividing line) -->
```

### Links
```html
<!-- External link -->
<a href="https://google.com">Visit Google</a>

<!-- Link opens in new tab -->
<a href="https://google.com" target="_blank">Google (new tab)</a>

<!-- Link to another page in your project -->
<a href="about.html">About Page</a>

<!-- Link to a section on the same page -->
<a href="#contact">Jump to Contact</a>
<section id="contact">Contact Section</section>
```

### Images
```html
<!-- Basic image -->
<img src="photo.jpg" alt="Description of the image" />

<!-- Image with size -->
<img src="logo.png" alt="Logo" width="200" height="100" />

<!-- Image from internet -->
<img src="https://example.com/image.png" alt="Online image" />
```

### Lists
```html
<!-- Unordered (bullet) list -->
<ul>
  <li>Apples</li>
  <li>Bananas</li>
  <li>Cherries</li>
</ul>

<!-- Ordered (numbered) list -->
<ol>
  <li>First step</li>
  <li>Second step</li>
  <li>Third step</li>
</ol>
```

### Tables
```html
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Age</th>
      <th>City</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Alex</td>
      <td>17</td>
      <td>New York</td>
    </tr>
    <tr>
      <td>Sam</td>
      <td>19</td>
      <td>Chicago</td>
    </tr>
  </tbody>
</table>
```

### Forms
```html
<form action="/submit" method="POST">

  <!-- Text input -->
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" placeholder="Your name" />

  <!-- Email input -->
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required />

  <!-- Password -->
  <input type="password" name="password" />

  <!-- Number -->
  <input type="number" name="age" min="1" max="120" />

  <!-- Dropdown -->
  <select name="country">
    <option value="us">United States</option>
    <option value="uk">United Kingdom</option>
  </select>

  <!-- Radio buttons -->
  <input type="radio" name="gender" value="male" /> Male
  <input type="radio" name="gender" value="female" /> Female

  <!-- Checkbox -->
  <input type="checkbox" name="terms" /> I agree to the terms

  <!-- Text area -->
  <textarea name="message" rows="5" cols="40"></textarea>

  <!-- Submit button -->
  <button type="submit">Send</button>

</form>
```

### Semantic Layout Tags (HTML5)
```html
<header>    <!-- Top of the page / navigation area -->
<nav>       <!-- Navigation menu -->
<main>      <!-- Main content -->
<section>   <!-- A section of content -->
<article>   <!-- Standalone piece of content -->
<aside>     <!-- Sidebar -->
<footer>    <!-- Bottom of the page -->

<!-- Non-semantic (for styling/layout) -->
<div>       <!-- Block-level container -->
<span>      <!-- Inline container -->
```

### Example Page Using Semantic HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>My Portfolio</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <header>
    <h1>Alex Johnson</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main>
    <section id="about">
      <h2>About Me</h2>
      <p>I'm a 17-year-old learning to code.</p>
    </section>

    <section id="projects">
      <h2>My Projects</h2>
      <article>
        <h3>Calculator App</h3>
        <p>A simple calculator built with HTML, CSS, and JavaScript.</p>
        <a href="#">View Project</a>
      </article>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Alex Johnson</p>
  </footer>

</body>
</html>
```

---

## HTML Attributes Cheat Sheet

| Attribute | Used On | What It Does |
|---|---|---|
| `href` | `<a>` | URL to link to |
| `src` | `<img>`, `<script>` | Source file path |
| `alt` | `<img>` | Text if image fails to load |
| `id` | Any | Unique identifier |
| `class` | Any | Group elements for CSS/JS |
| `style` | Any | Inline CSS styling |
| `type` | `<input>`, `<button>` | Input or button type |
| `placeholder` | `<input>` | Hint text inside input |
| `required` | `<input>` | Makes field mandatory |
| `disabled` | `<input>`, `<button>` | Grays out and disables element |
| `target="_blank"` | `<a>` | Opens link in new tab |

---

## Free Tutorials

- 🌐 **W3Schools HTML:** https://www.w3schools.com/html/
- 🌐 **MDN HTML Reference:** https://developer.mozilla.org/en-US/docs/Web/HTML
- 🎓 **freeCodeCamp Responsive Web Design:** https://www.freecodecamp.org/learn/2022/responsive-web-design/

---

## YouTube Tutorials

| Video | Description | Link |
|---|---|---|
| **freeCodeCamp** | HTML Full Course for Beginners (2hrs) | ![](https://www.youtube.com/watch?v=kUMe1FH4CHE) |
| **Traversy Media** | HTML Crash Course (1hr) | ![](https://www.youtube.com/watch?v=UB1O30fR-EE) |
| **Programming with Mosh** | HTML Tutorial for Beginners | ![](https://www.youtube.com/watch?v=qz0aGYrrlhU) |
| **Bro Code** | HTML Full Course | ![](https://www.youtube.com/watch?v=HD13eq_Pmp8) |

---

## Related Notes
- [[Coding - Master Index]]
- [[CSS]]
- [[JavaScript (JS)]]
- [[Beginner Stage]]
- [[Tools and Setup]]
