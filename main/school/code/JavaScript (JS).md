# JavaScript (JS)

> [!info] Quick Facts
> **Created:** 1995 by Brendan Eich at Netscape
> **Type:** High-level, interpreted, multi-paradigm programming language
> **Current Standard:** ECMAScript 2024 (ES15)
> **Used For:** Web interactivity, frontend frameworks, backend (Node.js), mobile apps
> **Difficulty:** ⭐⭐ — More complex than Python but essential for web
> **Runs In:** Every web browser; also server-side via [[Node.js]]
> **Official Reference:** https://developer.mozilla.org/en-US/docs/Web/JavaScript

---

**JavaScript** is the **only programming language that runs natively in web browsers**, making it the backbone of interactive web development. Every website you've ever clicked a button on, filled out a form on, or seen an animation on — JavaScript powered that interaction. With [[Node.js]], it also runs on servers, making it possible to use JavaScript for both frontend and backend development (full-stack).

---

## Why Learn JavaScript?

- **The language of the web** — unavoidable if you want to do anything with websites
- **Most in-demand language** in web development job postings
- **One language everywhere** — browser, server, mobile (React Native), desktop (Electron)
- **Massive ecosystem** — npm has over 2 million packages
- **Gateway to frameworks** — React, Vue, Angular, Next.js all require JS

---

## Core Syntax

### Variables
```javascript
// Three ways to declare variables:
var oldWay = "avoid this";      // function-scoped, outdated
let mutableVar = "can change";  // block-scoped, can reassign
const fixed = "can't change";   // block-scoped, can NOT reassign

let name = "Alex";
let age = 17;
let isStudent = true;
let nothing = null;
let notDefined = undefined;
```

### Strings
```javascript
let first = "Hello";
let last = "World";

// Concatenation
let full = first + " " + last;

// Template literals (modern, preferred)
let message = `My name is ${name} and I am ${age} years old.`;

// String methods
"hello".toUpperCase();      // "HELLO"
"  hello  ".trim();         // "hello"
"hello world".split(" ");   // ["hello", "world"]
"hello".includes("ell");    // true
```

### Functions
```javascript
// Regular function
function add(a, b) {
  return a + b;
}

// Arrow function (modern shorthand)
const multiply = (a, b) => a * b;

// Default parameters
const greet = (name = "stranger") => `Hello, ${name}!`;

// Callback function
const numbers = [1, 2, 3, 4, 5];
numbers.forEach(n => console.log(n));
```

### Arrays
```javascript
const fruits = ["apple", "banana", "cherry"];

// Access
console.log(fruits[0]);       // "apple"
console.log(fruits.length);   // 3

// Modify
fruits.push("mango");         // add to end
fruits.pop();                 // remove from end
fruits.unshift("grape");      // add to beginning

// Powerful array methods
const doubled = fruits.map(f => f.toUpperCase());
const long = fruits.filter(f => f.length > 5);
const found = fruits.find(f => f.startsWith("b"));
const hasApple = fruits.includes("apple");   // true
```

### Objects
```javascript
const person = {
  name: "Alex",
  age: 17,
  hobbies: ["coding", "gaming"],
  address: {
    city: "New York",
    zip: "10001"
  },
  greet() {
    return `Hi, I'm ${this.name}`;
  }
};

// Access
console.log(person.name);            // "Alex"
console.log(person["age"]);          // 17
console.log(person.address.city);    // "New York"
console.log(person.greet());         // "Hi, I'm Alex"

// Destructuring
const { name, age } = person;
const { city } = person.address;
```

### Conditionals and Loops
```javascript
// If/else
if (age >= 18) {
  console.log("Adult");
} else if (age >= 13) {
  console.log("Teenager");
} else {
  console.log("Child");
}

// Ternary operator
const label = age >= 18 ? "Adult" : "Minor";

// For loop
for (let i = 0; i < 5; i++) {
  console.log(i);
}

// For...of (iterating arrays)
for (const fruit of fruits) {
  console.log(fruit);
}

// For...in (iterating object keys)
for (const key in person) {
  console.log(key, person[key]);
}
```

### Async JavaScript
```javascript
// Promises
fetch("https://api.example.com/data")
  .then(res => res.json())
  .then(data => console.log(data))
  .catch(err => console.error(err));

// Async/Await (cleaner syntax, same thing)
async function getData() {
  try {
    const response = await fetch("https://api.example.com/data");
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error("Failed:", error);
  }
}
```

### DOM Manipulation (Making Web Pages Interactive)
```javascript
// Select elements
const button = document.querySelector("#myButton");
const heading = document.querySelector("h1");
const allParagraphs = document.querySelectorAll("p");

// Change content
heading.textContent = "New Heading";
heading.innerHTML = "<span>Bold</span> Heading";

// Change styles
heading.style.color = "red";
heading.classList.add("active");
heading.classList.remove("inactive");

// Event listeners
button.addEventListener("click", () => {
  alert("Button clicked!");
  heading.textContent = "You clicked the button!";
});

// Create and add new elements
const newParagraph = document.createElement("p");
newParagraph.textContent = "This was added by JavaScript.";
document.body.appendChild(newParagraph);
```

---

## ES6+ Modern Features (Must Know)

```javascript
// Spread operator
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5];  // [1, 2, 3, 4, 5]

const obj1 = { a: 1 };
const obj2 = { ...obj1, b: 2 };  // { a: 1, b: 2 }

// Optional chaining (avoid undefined errors)
const city = user?.address?.city;  // undefined instead of error

// Nullish coalescing
const name = user.name ?? "Anonymous";  // use "Anonymous" if null/undefined

// Modules
export const PI = 3.14159;
export function circle(r) { return PI * r * r; }

import { PI, circle } from "./math.js";
```

---

## Learning Path

| Level | Topics |
|---|---|
| **Beginner** | Variables, functions, loops, DOM, events |
| **Amateur** | Arrays methods, async/await, fetch API, ES6+ |
| **Master** | Closures, prototypes, event loop, TypeScript, frameworks |

---

## Free Tutorials

- 🌐 **MDN Web Docs (the official reference):** https://developer.mozilla.org/en-US/docs/Web/JavaScript
- 🌐 **The Modern JavaScript Tutorial:** https://javascript.info/
- 🌐 **W3Schools JS:** https://www.w3schools.com/js/
- 🎓 **freeCodeCamp JavaScript Algorithms:** https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/
- 🎓 **The Odin Project:** https://www.theodinproject.com/

---

## YouTube Tutorials

| Video / Channel           | Description                                 | Link                                             |
| ------------------------- | ------------------------------------------- | ------------------------------------------------ |
| **freeCodeCamp**          | JavaScript Full Course for Beginners (8hrs) | ![](https://www.youtube.com/watch?v=PkZNo7MFNFg) |
| **Traversy Media**        | JavaScript Crash Course                     | ![](https://www.youtube.com/watch?v=hdI2bqOjy3c) |
| **Programming with Mosh** | JavaScript Tutorial for Beginners (1hr)     | ![](https://www.youtube.com/watch?v=W6NZfCO5SIk) |
| **Fireship**              | JavaScript in 100 Seconds                   | ![](https://www.youtube.com/watch?v=DHjqpvDnNGE) |
| **Traversy Media**        | Async JS Crash Course                       | ![](https://www.youtube.com/watch?v=PoRJizFvM7s) |

---

## Related Notes
- [[Coding - Master Index]]
- [[HTML]]
- [[CSS]]
- [[TypeScript]]
- [[React]]
- [[Node.js]]
- [[Beginner Stage]]
- [[Amateur Stage]]
- [[Master Stage]]
