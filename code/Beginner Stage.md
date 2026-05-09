# Beginner Stage — Zero to Writing Real Code

> [!info] Who This Is For
> You have **never written code before** — or you've tried and given up. This stage takes you from complete zero to being able to build simple web pages and write basic programs. Estimated time: **4–8 weeks** at 30–60 min/day.

---

## Contents
1. [[#The Right Mindset]]
2. [[#Setting Up Your Computer]]
3. [[#Stage 1 — HTML]]
4. [[#Stage 2 — CSS]]
5. [[#Stage 3 — Basic JavaScript]]
6. [[#Stage 4 — Basic Python]]
7. [[#Beginner Projects to Build]]
8. [[#Beginner YouTube Playlist]]
9. [[#Beginner Websites]]
10. [[#How to Know You're Ready for the Next Stage]]

---

## The Right Mindset

> [!info] Read This First
> Learning to code is **not about being smart** — it's about being patient and consistent. Every professional developer was once exactly where you are. The difference is they kept going when it got confusing.
>
> **Expect this:** You will get error messages. Your code will not work. You will feel stupid. This is not failure — this is literally how coding works. The skill you're building is not "write perfect code" — it's "read an error and figure out what's wrong."

Rules for beginners:
- **Never copy-paste code you're learning** — type it out letter by letter
- **Read error messages** — they tell you exactly what went wrong
- **Search everything** — "how do I make a button in HTML" is a perfectly professional question
- **Build something every day**, even if it's tiny
- **Don't jump ahead** — each stage exists for a reason

---

## Setting Up Your Computer

Before writing code you need two things:

### 1. A Code Editor

> [!info] Install VS Code
> **Visual Studio Code (VS Code)** is the most popular free code editor in the world. It's what most professionals use.
> - **Download:** https://code.visualstudio.com/
> - Install the extension **"Live Server"** so you can see your HTML/CSS changes instantly in your browser
> - Install **"Prettier"** for auto-formatting

### 2. A Browser

Use **Google Chrome** or **Firefox** — both have built-in developer tools (right-click → "Inspect") that let you see and debug your code.

### 3. A GitHub Account (Free)

Sign up at https://github.com — you'll use this to save and share your code. See [[Git and GitHub]].

---

## Stage 1 — HTML

> [!info] What is HTML?
> **HTML (HyperText Markup Language)** is the skeleton of every web page. It defines structure — headings, paragraphs, images, links, buttons. It is **not** a programming language — it's a markup language. It's the easiest thing to learn and the best starting point because you see results immediately.
> Full note: **[[HTML]]**

### What You'll Learn
- Tags and elements (`<h1>`, `<p>`, `<a>`, `<img>`, `<div>`)
- How to structure a web page
- Links, images, lists, tables, forms

### Beginner HTML Example
```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Hello, World!</h1>
    <p>This is my first web page.</p>
    <a href="https://google.com">Click here</a>
  </body>
</html>
```

### HTML Resources
- 🌐 **W3Schools HTML Tutorial:** https://www.w3schools.com/html/
- 🎓 **freeCodeCamp Responsive Web Design:** https://www.freecodecamp.org/learn/2022/responsive-web-design/
- 📺 **YouTube — HTML Full Course (freeCodeCamp, 2hrs):** https://www.youtube.com/watch?v=kUMe1FH4CHE
![](https://www.youtube.com/watch?v=kUMe1FH4CHE)
- 📺 **YouTube — HTML Crash Course (Traversy Media, 1hr):** https://www.youtube.com/watch?v=UB1O30fR-EE
![](https://www.youtube.com/watch?v=UB1O30fR-EE)

### HTML Milestone
✅ Build a simple webpage with your name, a photo, a paragraph about yourself, and a list of your hobbies.

---

## Stage 2 — CSS

> [!info] What is CSS?
> **CSS (Cascading Style Sheets)** makes web pages look good. It controls colors, fonts, layouts, spacing, animations, and everything visual. HTML is the skeleton — CSS is the skin.
> Full note: **[[CSS]]**

### What You'll Learn
- Selectors, properties, values
- Colors, fonts, backgrounds
- The box model (margin, padding, border)
- Flexbox and Grid (page layouts)
- Responsive design (works on phones and desktops)

### Beginner CSS Example
```css
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}

h1 {
  color: navy;
  text-align: center;
}

p {
  font-size: 18px;
  line-height: 1.6;
}
```

### CSS Resources
- 🌐 **W3Schools CSS Tutorial:** https://www.w3schools.com/css/
- 🎓 **freeCodeCamp CSS:** https://www.freecodecamp.org/learn/2022/responsive-web-design/
- 📺 **YouTube — CSS Full Course (freeCodeCamp, 11hrs):** https://www.youtube.com/watch?v=OXGznpKZ_sA
![](https://www.youtube.com/watch?v=OXGznpKZ_sA)
- 📺 **YouTube — CSS Crash Course (Traversy Media, 1.5hrs):** https://www.youtube.com/watch?v=yfoY53QXEnI
![](https://www.youtube.com/watch?v=yfoY53QXEnI)
- 📺 **YouTube — Flexbox in 15 Minutes (Web Dev Simplified):** https://www.youtube.com/watch?v=fYq5PXgSsbE
![](https://www.youtube.com/watch?v=fYq5PXgSsbE)

### CSS Milestone
✅ Take your HTML page from Stage 1 and style it — add colors, fonts, and center your content using Flexbox.

---

## Stage 3 — Basic JavaScript

> [!info] What is JavaScript?
> **JavaScript (JS)** makes web pages interactive. Button clicks, pop-ups, animations, form validation, fetching data — all JS. It is a real programming language with logic, variables, functions, and loops.
> Full note: **[[JavaScript (JS)]]**

### What You'll Learn (Beginner JS)
- Variables (`let`, `const`)
- Data types (strings, numbers, booleans)
- Functions
- If/else statements
- Loops (`for`, `while`)
- Selecting and changing HTML with JS (`document.querySelector`)
- Events (click, hover, submit)

### Beginner JS Example
```javascript
// Variables
let name = "Alex";
let age = 17;

// Function
function greet(person) {
  return "Hello, " + person + "!";
}

// If/else
if (age >= 18) {
  console.log("You are an adult.");
} else {
  console.log("You are a minor.");
}

// Loop
for (let i = 1; i <= 5; i++) {
  console.log("Number: " + i);
}
```

### JavaScript Beginner Resources
- 🌐 **W3Schools JS Tutorial:** https://www.w3schools.com/js/
- 🎓 **freeCodeCamp JS Algorithms & Data Structures:** https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/
- 📺 **YouTube — JavaScript Full Course for Beginners (freeCodeCamp, 8hrs):** https://www.youtube.com/watch?v=PkZNo7MFNFg
![](https://www.youtube.com/watch?v=PkZNo7MFNFg)
- 📺 **YouTube — JavaScript Crash Course (Traversy Media, 1.5hrs):** https://www.youtube.com/watch?v=hdI2bqOjy3c
![](https://www.youtube.com/watch?v=hdI2bqOjy3c)
- 📺 **YouTube — JavaScript Tutorial for Beginners (Programming with Mosh, 1hr):** https://www.youtube.com/watch?v=W6NZfCO5SIk
![](https://www.youtube.com/watch?v=W6NZfCO5SIk)

### JavaScript Milestone
✅ Build a button on your HTML page that, when clicked, changes the text of a paragraph using JavaScript.

---

## Stage 4 — Basic Python

> [!info] What is Python?
> **Python** is the most beginner-friendly full programming language. It reads almost like English. It's used in AI, data science, web development, automation, scripting — virtually everything. Learning it solidifies your understanding of programming logic.
> Full note: **[[Python]]**

### What You'll Learn (Beginner Python)
- Print statements and input
- Variables and data types
- String manipulation
- Lists and dictionaries
- For and while loops
- Functions
- Reading and writing files
- Basic error handling

### Beginner Python Example
```python
# Variables and print
name = input("What is your name? ")
print("Hello, " + name + "!")

# List and loop
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

# Function
def add_numbers(a, b):
    return a + b

result = add_numbers(5, 3)
print("5 + 3 =", result)
```

### Python Beginner Resources
- 🌐 **W3Schools Python Tutorial:** https://www.w3schools.com/python/
- 🎓 **freeCodeCamp Python:** https://www.freecodecamp.org/learn/scientific-computing-with-python/
- 🎓 **Harvard CS50P (free, beginner Python):** https://cs50.harvard.edu/python/
- 📺 **YouTube — Python Tutorial for Beginners (Programming with Mosh, 6hrs):** https://www.youtube.com/watch?v=_uQrJ0TkZlc
![](https://www.youtube.com/watch?v=_uQrJ0TkZlc)
- 📺 **YouTube — Python Full Course (freeCodeCamp, 4.5hrs):** https://www.youtube.com/watch?v=rfscVS0vtbw
![](https://www.youtube.com/watch?v=rfscVS0vtbw)
- 📺 **YouTube — Python Beginner Tutorial Series (Corey Schafer):** https://www.youtube.com/playlist?list=PL-osiE80TeTskrapNbzXhwoFUiLCjGgY7
- 📺 **YouTube — Python for Beginners (Tech with Tim):** https://www.youtube.com/watch?v=sxTmJE4k0ho
![](https://www.youtube.com/watch?v=sxTmJE4k0ho)

### Python Milestone
✅ Build a simple number guessing game — the program picks a random number, and the user guesses until they get it right.

---

## Beginner Projects to Build

> [!info] Why Projects Matter
> Tutorials teach you syntax. Projects teach you to **think like a programmer**. Build at least one project per stage before moving on.

| Project | Languages | What You Learn |
|---|---|---|
| Personal profile page | HTML + CSS | Structure, styling, layout |
| Styled portfolio page | HTML + CSS | Flexbox, responsive design |
| To-do list | HTML + CSS + JS | DOM manipulation, events |
| Calculator | HTML + CSS + JS | Functions, logic |
| Number guessing game | Python | Loops, conditionals, input |
| Simple quiz app | Python | Lists, functions, logic |
| Rock Paper Scissors | Python or JS | Random, conditionals |

---

## Beginner YouTube Playlist

| Channel | Best For | Link |
|---|---|---|
| **freeCodeCamp** | Complete free courses, all languages | ![](https://www.youtube.com/@freecodecamp) |
| **Programming with Mosh** | Clean, beginner-friendly Python & JS | ![](https://www.youtube.com/@programmingwithmosh) |
| **Traversy Media** | HTML, CSS, JS crash courses | ![](https://www.youtube.com/@TraversyMedia) |
| **Web Dev Simplified** | CSS, JS fundamentals explained clearly | ![](https://www.youtube.com/@WebDevSimplified) |
| **CS Dojo** | Python + programming fundamentals | ![](https://www.youtube.com/@CSDojo) |

---

## Beginner Websites

| Site | What It Does | Link |
|---|---|---|
| **W3Schools** | Fast reference + try-it editor | https://www.w3schools.com |
| **freeCodeCamp** | Free full curriculum with certifications | https://www.freecodecamp.org |
| **Khan Academy** | Visual, browser-based beginner coding | https://www.khanacademy.org/computing |
| **Codecademy** | Interactive step-by-step lessons | https://www.codecademy.com |
| **CS50 (Harvard, free)** | Best free university-level intro to CS | https://cs50.harvard.edu/x/ |

---

## How to Know You're Ready for the Next Stage

✅ You can build a basic HTML/CSS web page from scratch without looking up every tag
✅ You can make a button do something with JavaScript
✅ You can write a Python program that uses loops, functions, and conditionals
✅ You understand what a variable, function, and loop are without having to look them up
✅ You've built at least 2 projects on your own (not following a tutorial step by step)

**When all 5 are true → move to [[Amateur Stage]]**

---

## Related Notes
- [[Coding - Master Index]]
- [[Amateur Stage]]
- [[Master Stage]]
- [[HTML]]
- [[CSS]]
- [[JavaScript (JS)]]
- [[Python]]
- [[Tools and Setup]]
- [[YouTube Channels for Coding]]
