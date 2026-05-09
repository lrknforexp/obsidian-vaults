# CSS

> [!info] Quick Facts
> **Full Name:** Cascading Style Sheets
> **Created:** 1996 by Håkon Wium Lie
> **Current Version:** CSS3 (with continuous modules)
> **Type:** Stylesheet language
> **Used For:** Visual design and layout of web pages
> **Difficulty:** ⭐ to ⭐⭐⭐ — Easy to start, takes time to master
> **Official Reference:** https://developer.mozilla.org/en-US/docs/Web/CSS

---

**CSS** makes web pages look good. While [[HTML]] defines the structure (what's on the page), CSS defines the presentation — colors, fonts, spacing, layout, animations, and everything visual. Without CSS, every website would be plain black text on a white background.

---

## How CSS Works

CSS is applied to HTML elements using **selectors** and **rules**:

```css
selector {
  property: value;
  property: value;
}
```

**Three ways to add CSS to an HTML page:**

```html
<!-- 1. External stylesheet (best practice) -->
<link rel="stylesheet" href="style.css" />

<!-- 2. Internal style block -->
<style>
  h1 { color: red; }
</style>

<!-- 3. Inline style (use sparingly) -->
<h1 style="color: red;">Hello</h1>
```

---

## Selectors

```css
/* Element selector — targets all <p> tags */
p { color: gray; }

/* Class selector — targets elements with class="card" */
.card { background: white; }

/* ID selector — targets element with id="header" */
#header { background: navy; }

/* Multiple selectors */
h1, h2, h3 { font-family: sans-serif; }

/* Descendant — <p> inside a .container */
.container p { color: blue; }

/* Direct child */
.nav > li { display: inline; }

/* Hover state */
button:hover { background: darkblue; }

/* First child */
li:first-child { font-weight: bold; }

/* Nth child */
tr:nth-child(even) { background: #f5f5f5; }
```

---

## Colors

```css
/* Named colors */
color: red;
color: navy;
color: transparent;

/* Hex codes */
color: #ff0000;       /* red */
color: #1a1a2e;       /* dark navy */
color: #fff;          /* white (shorthand) */

/* RGB */
color: rgb(255, 0, 0);
color: rgb(26, 26, 46);

/* RGBA (with transparency) */
color: rgba(0, 0, 0, 0.5);   /* 50% transparent black */

/* HSL (hue, saturation, lightness) */
color: hsl(240, 100%, 50%);  /* blue */
```

---

## Text and Typography

```css
h1 {
  font-family: "Georgia", serif;       /* font stack */
  font-size: 48px;                     /* or rem, em, % */
  font-weight: bold;                   /* or 100-900 */
  font-style: italic;
  color: #1a1a2e;
  text-align: center;                  /* left, right, justify */
  text-transform: uppercase;
  text-decoration: underline;
  letter-spacing: 2px;
  line-height: 1.6;                    /* 1.6 × font-size */
}

/* Google Fonts — add to <head> first */
/* <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet"> */
font-family: "Poppins", sans-serif;
```

---

## The Box Model

> [!info] The Box Model
> Every HTML element is a box. The box has four layers:
> - **Content** — the actual text or image
> - **Padding** — space inside the border, around the content
> - **Border** — the line around the element
> - **Margin** — space outside the border, between elements

```css
.box {
  width: 300px;
  height: 200px;
  padding: 20px;             /* all sides */
  padding: 10px 20px;        /* top/bottom | left/right */
  margin: 10px auto;         /* center horizontally */
  border: 2px solid black;
  border-radius: 8px;        /* rounded corners */
  box-sizing: border-box;    /* include padding in width (recommended) */
}
```

---

## Flexbox (1D Layout)

> [!info] Flexbox
> Flexbox arranges items in a **row or column**. It's the best way to center things and build simple layouts.

```css
.container {
  display: flex;
  flex-direction: row;       /* or column */
  justify-content: center;   /* horizontal: flex-start, flex-end, space-between, space-around */
  align-items: center;       /* vertical: flex-start, flex-end, stretch */
  gap: 16px;                 /* space between children */
  flex-wrap: wrap;           /* allow wrapping to next row */
}

/* Center anything perfectly */
.center {
  display: flex;
  justify-content: center;
  align-items: center;
}

/* Flex children */
.item {
  flex: 1;                   /* grow to fill equal space */
  flex: 0 0 200px;           /* fixed 200px width, don't grow/shrink */
}
```

---

## CSS Grid (2D Layout)

> [!info] CSS Grid
> Grid arranges items in **rows AND columns** simultaneously — best for page-level layouts.

```css
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;        /* 3 equal columns */
  grid-template-columns: 200px 1fr 1fr;      /* fixed + flexible */
  grid-template-columns: repeat(3, 1fr);     /* same as first */
  grid-template-rows: auto;
  gap: 24px;
}

/* Spanning multiple cells */
.wide-item {
  grid-column: span 2;     /* takes up 2 columns */
  grid-row: span 2;        /* takes up 2 rows */
}

/* Named grid areas */
.layout {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
  grid-template-columns: 250px 1fr;
}

.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main { grid-area: main; }
.footer { grid-area: footer; }
```

---

## Responsive Design

```css
/* Mobile-first approach: start small, expand for larger screens */

/* Base styles (mobile) */
.container {
  width: 100%;
  padding: 16px;
}

/* Tablet (768px and up) */
@media (min-width: 768px) {
  .container {
    max-width: 720px;
    margin: 0 auto;
  }
}

/* Desktop (1024px and up) */
@media (min-width: 1024px) {
  .container {
    max-width: 1200px;
  }
}

/* Breakpoint cheat sheet */
/* Mobile: < 768px */
/* Tablet: 768px – 1024px */
/* Desktop: > 1024px */
```

---

## CSS Variables (Custom Properties)

```css
:root {
  --primary: #4f46e5;
  --secondary: #7c3aed;
  --text: #1f2937;
  --bg: #ffffff;
  --radius: 8px;
  --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.button {
  background: var(--primary);
  color: white;
  border-radius: var(--radius);
  box-shadow: var(--shadow);
}

.button:hover {
  background: var(--secondary);
}
```

---

## Transitions and Animations

```css
/* Smooth transitions */
button {
  background: blue;
  transition: background 0.3s ease, transform 0.2s ease;
}

button:hover {
  background: darkblue;
  transform: scale(1.05);
}

/* Keyframe animations */
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.card {
  animation: fadeIn 0.5s ease forwards;
}

@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.loader {
  animation: spin 1s linear infinite;
}
```

---

## CSS Units Cheat Sheet

| Unit | Description | When to Use |
|---|---|---|
| `px` | Pixels — fixed size | Borders, precise sizing |
| `%` | Percentage of parent | Responsive widths |
| `em` | Relative to current font size | Font-relative spacing |
| `rem` | Relative to root font size | Font sizes (best practice) |
| `vw` | % of viewport width | Full-width sections |
| `vh` | % of viewport height | Full-height sections |
| `fr` | Fraction of grid space | CSS Grid columns/rows |

---

## Free Tutorials

- 🌐 **W3Schools CSS:** https://www.w3schools.com/css/
- 🌐 **MDN CSS Reference:** https://developer.mozilla.org/en-US/docs/Web/CSS
- 🌐 **CSS Tricks:** https://css-tricks.com/
- 🎓 **freeCodeCamp Responsive Web Design:** https://www.freecodecamp.org/learn/2022/responsive-web-design/

---

## YouTube Tutorials

| Video | Description | Link |
|---|---|---|
| **freeCodeCamp** | CSS Full Course for Beginners (11hrs) | ![](https://www.youtube.com/watch?v=OXGznpKZ_sA) |
| **Traversy Media** | CSS Crash Course | ![](https://www.youtube.com/watch?v=yfoY53QXEnI) |
| **Kevin Powell** | CSS is Easy (beginner series) | ![](https://www.youtube.com/@KevinPowell) |
| **Web Dev Simplified** | Flexbox in 15 Minutes | ![](https://www.youtube.com/watch?v=fYq5PXgSsbE) |
| **Traversy Media** | CSS Grid Crash Course | ![](https://www.youtube.com/watch?v=jV8B24rSN5o) |
| **Kevin Powell** | CSS Animations Tutorial | ![](https://www.youtube.com/watch?v=YszONjKpgg4) |

---

## Related Notes
- [[Coding - Master Index]]
- [[HTML]]
- [[JavaScript (JS)]]
- [[React]]
- [[Beginner Stage]]
- [[Amateur Stage]]
