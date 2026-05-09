# Amateur Stage — Building Real Things

> [!info] Who This Is For
> You've completed the [[Beginner Stage]] — you can write basic HTML, CSS, JS, and Python. Now you learn to build **real, complete projects** and start working like an actual developer. Estimated time: **2–4 months** at 1hr/day.

---

## Contents
1. [[#What Changes at This Stage]]
2. [[#JavaScript — Going Deeper]]
3. [[#Python — Going Deeper]]
4. [[#CSS — Intermediate Skills]]
5. [[#SQL and Databases]]
6. [[#Git and GitHub]]
7. [[#Introduction to React]]
8. [[#Introduction to Node.js]]
9. [[#Amateur Projects to Build]]
10. [[#Amateur YouTube Resources]]
11. [[#How to Know You're Ready for the Next Stage]]

---

## What Changes at This Stage

> [!info] The Shift
> At the beginner stage, you followed tutorials. At the amateur stage, you **use tutorials as references** but build your own things. The difference is huge.
>
> You'll hit walls — problems where you don't know what to do. That's normal. The skill you're developing now is: **"I don't know how to do this yet — how do I figure it out?"**
>
> The answer is always: search it, read the error, try things, and piece it together. That is literally what every working developer does every day.

Key habits to build now:
- Use **[[Git and GitHub]]** for every project — never lose code again
- Read **documentation** (official docs for every language and library)
- Write **comments** in your code explaining what each section does
- Start building a **portfolio** on GitHub

---

## JavaScript — Going Deeper

> [!info] Intermediate JS Topics
> Full note: **[[JavaScript (JS)]]**

### Topics to Learn

**Arrays and Array Methods**
```javascript
const numbers = [1, 2, 3, 4, 5];

// map - transform every item
const doubled = numbers.map(n => n * 2); // [2, 4, 6, 8, 10]

// filter - keep items that match condition
const evens = numbers.filter(n => n % 2 === 0); // [2, 4]

// reduce - collapse to a single value
const sum = numbers.reduce((acc, n) => acc + n, 0); // 15
```

**Objects**
```javascript
const person = {
  name: "Alex",
  age: 17,
  greet: function() {
    return "Hi, I'm " + this.name;
  }
};
console.log(person.greet()); // "Hi, I'm Alex"
```

**Fetch API (Getting data from the internet)**
```javascript
fetch("https://api.example.com/data")
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error("Error:", error));
```

**ES6+ Modern Syntax**
```javascript
// Arrow functions
const add = (a, b) => a + b;

// Destructuring
const { name, age } = person;

// Template literals
const message = `Hello, ${name}! You are ${age} years old.`;

// Async/Await (cleaner than .then())
async function getData() {
  const response = await fetch("https://api.example.com/data");
  const data = await response.json();
  return data;
}
```

### Intermediate JS Resources
- 🌐 **The Modern JavaScript Tutorial:** https://javascript.info/
- 📺 **YouTube — JavaScript DOM Crash Course (Traversy Media):** https://www.youtube.com/watch?v=0ik6X4DJKCc
![](https://www.youtube.com/watch?v=0ik6X4DJKCc)
- 📺 **YouTube — Async JS Crash Course (Traversy Media):** https://www.youtube.com/watch?v=PoRJizFvM7s
![](https://www.youtube.com/watch?v=PoRJizFvM7s)
- 📺 **YouTube — JavaScript Intermediate Tutorial (Web Dev Simplified):** https://www.youtube.com/watch?v=R9I85RhI7Cg
![](https://www.youtube.com/watch?v=R9I85RhI7Cg)
- 📺 **YouTube — JavaScript Full Course (Fireship, advanced concepts fast):** https://www.youtube.com/watch?v=jS4aFq5-91M
![](https://www.youtube.com/watch?v=jS4aFq5-91M)

---

## Python — Going Deeper

> [!info] Intermediate Python Topics
> Full note: **[[Python]]**

### Topics to Learn

**Object-Oriented Programming (OOP)**
```python
class Animal:
    def __init__(self, name, species):
        self.name = name
        self.species = species

    def speak(self):
        return f"{self.name} makes a sound."

class Dog(Animal):
    def speak(self):
        return f"{self.name} barks!"

dog = Dog("Rex", "Canis lupus familiaris")
print(dog.speak())  # "Rex barks!"
```

**File Handling**
```python
# Writing to a file
with open("data.txt", "w") as f:
    f.write("Hello, file!")

# Reading from a file
with open("data.txt", "r") as f:
    content = f.read()
    print(content)
```

**Libraries (install with pip)**
```python
# requests - make HTTP calls
import requests
response = requests.get("https://api.github.com")
print(response.json())

# pandas - work with data tables
import pandas as pd
df = pd.read_csv("data.csv")
print(df.head())
```

### Intermediate Python Resources
- 📺 **YouTube — Intermediate Python (Corey Schafer playlist):** https://www.youtube.com/playlist?list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU
- 📺 **YouTube — OOP in Python (Tech with Tim):** https://www.youtube.com/watch?v=JeznW_7DlB0
![](https://www.youtube.com/watch?v=JeznW_7DlB0)
- 📺 **YouTube — Python Automation (freeCodeCamp):** https://www.youtube.com/watch?v=s8XjEuplx_U
![](https://www.youtube.com/watch?v=s8XjEuplx_U)
- 🌐 **Real Python (project-based tutorials):** https://realpython.com/

---

## CSS — Intermediate Skills

### Topics to Learn
- **Flexbox** — one-dimensional layouts (rows or columns)
- **CSS Grid** — two-dimensional layouts (rows AND columns)
- **CSS Variables** (`--primary-color: blue;`)
- **Transitions and Animations** (`transition`, `@keyframes`)
- **Responsive Design** — mobile-first with `@media` queries
- **Pseudo-classes** (`:hover`, `:focus`, `:nth-child`)

```css
/* CSS Variables */
:root {
  --primary: #4f46e5;
  --text: #1f2937;
}

/* Grid Layout */
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

/* Animation */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

.card {
  animation: fadeIn 0.4s ease;
}

/* Media Query */
@media (max-width: 768px) {
  .container {
    grid-template-columns: 1fr;
  }
}
```

### CSS Intermediate Resources
- 📺 **YouTube — CSS Grid Crash Course (Traversy Media):** https://www.youtube.com/watch?v=jV8B24rSN5o
![](https://www.youtube.com/watch?v=jV8B24rSN5o)
- 📺 **YouTube — CSS Animations (Kevin Powell):** https://www.youtube.com/watch?v=YszONjKpgg4
![](https://www.youtube.com/watch?v=YszONjKpgg4)
- 📺 **YouTube — Responsive Design (Web Dev Simplified):** https://www.youtube.com/watch?v=yU7jJ3NbPdA
![](https://www.youtube.com/watch?v=yU7jJ3NbPdA)
- 🌐 **CSS Tricks (best CSS reference site):** https://css-tricks.com/

---

## SQL and Databases

> [!info] What is SQL?
> **SQL (Structured Query Language)** is how you talk to databases. Almost every real app stores data — user accounts, posts, orders, messages — and SQL is how you retrieve and manage it.
> Full note: **[[SQL]]**

### Core SQL Commands
```sql
-- Select data
SELECT name, age FROM users WHERE age > 18;

-- Insert data
INSERT INTO users (name, age, email) VALUES ('Alex', 17, 'alex@email.com');

-- Update data
UPDATE users SET age = 18 WHERE name = 'Alex';

-- Delete data
DELETE FROM users WHERE name = 'Alex';

-- Join two tables
SELECT orders.id, users.name
FROM orders
JOIN users ON orders.user_id = users.id;
```

### SQL Resources
- 🌐 **W3Schools SQL Tutorial:** https://www.w3schools.com/sql/
- 🎓 **SQLZoo (interactive SQL practice):** https://sqlzoo.net/
- 📺 **YouTube — SQL Full Course (freeCodeCamp, 4hrs):** https://www.youtube.com/watch?v=HXV3zeQKqGY
![](https://www.youtube.com/watch?v=HXV3zeQKqGY)
- 📺 **YouTube — SQL Crash Course (Traversy Media):** https://www.youtube.com/watch?v=9ylj9NR0Lcg
![](https://www.youtube.com/watch?v=9ylj9NR0Lcg)

---

## Git and GitHub

> [!info] Why Git is Non-Negotiable
> **[[Git and GitHub]]** is version control — it tracks every change you make to your code so you can undo mistakes, collaborate with others, and show your work to employers. Every professional developer uses it daily.

### Core Git Commands
```bash
git init                    # Start tracking a folder
git add .                   # Stage all changes
git commit -m "My message"  # Save a snapshot
git push origin main        # Upload to GitHub
git pull                    # Download latest changes
git branch new-feature      # Create a new branch
git checkout new-feature    # Switch to that branch
git merge new-feature       # Merge branch into main
```

### Git Resources
- 📺 **YouTube — Git and GitHub for Beginners (freeCodeCamp, 1hr):** https://www.youtube.com/watch?v=RGOj5yH7evk
![](https://www.youtube.com/watch?v=RGOj5yH7evk)
- 📺 **YouTube — Git Crash Course (Traversy Media):** https://www.youtube.com/watch?v=SWYqp7iY_Tc
![](https://www.youtube.com/watch?v=SWYqp7iY_Tc)
- 🌐 **GitHub Docs:** https://docs.github.com/

---

## Introduction to React

> [!info] What is React?
> **[[React]]** is a JavaScript library for building user interfaces. Instead of writing raw HTML + JS, you write **components** — reusable pieces of UI. It's the most in-demand frontend skill in the job market.

### Basic React Component
```jsx
import { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <h1>Count: {count}</h1>
      <button onClick={() => setCount(count + 1)}>Add 1</button>
    </div>
  );
}

export default Counter;
```

### React Resources
- 🌐 **Official React Docs (best starting point):** https://react.dev/
- 📺 **YouTube — React Course for Beginners (freeCodeCamp, 12hrs):** https://www.youtube.com/watch?v=bMknfKXIFA8
![](https://www.youtube.com/watch?v=bMknfKXIFA8)
- 📺 **YouTube — React JS Crash Course (Traversy Media):** https://www.youtube.com/watch?v=w7ejDZ8SWv8
![](https://www.youtube.com/watch?v=w7ejDZ8SWv8)
- 📺 **YouTube — React Tutorial (Web Dev Simplified):** https://www.youtube.com/watch?v=Rh3tobg7hEo
![](https://www.youtube.com/watch?v=Rh3tobg7hEo)

---

## Introduction to Node.js

> [!info] What is Node.js?
> **[[Node.js]]** lets you run JavaScript on a server (not just in the browser). It's used to build backends, REST APIs, and full-stack applications.

### Basic Node.js Server
```javascript
const http = require("http");

const server = http.createServer((req, res) => {
  res.writeHead(200, { "Content-Type": "text/plain" });
  res.end("Hello from my server!");
});

server.listen(3000, () => {
  console.log("Server running at http://localhost:3000");
});
```

### Node.js Resources
- 📺 **YouTube — Node.js Crash Course (Traversy Media):** https://www.youtube.com/watch?v=fBNz5xF-Kx4
![](https://www.youtube.com/watch?v=fBNz5xF-Kx4)
- 📺 **YouTube — Node.js Full Course (Net Ninja):** https://www.youtube.com/playlist?list=PL4cUxeGkcC9jszmQoUKCtkq3NH3yEMnDm
- 🌐 **Node.js Official Docs:** https://nodejs.org/en/docs/

---

## Amateur Projects to Build

| Project | Stack | Skills Practiced |
|---|---|---|
| Responsive portfolio website | HTML + CSS + JS | Grid, Flexbox, responsive |
| Weather app (using a real API) | JS + Fetch API | APIs, async, JSON |
| To-do app with localStorage | HTML + CSS + JS | DOM, storage, events |
| Movie search app | JS + React | Components, state, API |
| Python web scraper | Python + BeautifulSoup | Libraries, data handling |
| Simple blog (backend) | Node.js + Express | Server, routing, HTTP |
| SQL database app | Python + SQLite | Database CRUD |
| Discord or Telegram bot | Python | Libraries, APIs, automation |

---

## Amateur YouTube Resources

| Channel | Best For | Link |
|---|---|---|
| **Traversy Media** | All-around web dev — best crash courses | ![](https://www.youtube.com/@TraversyMedia) |
| **Web Dev Simplified** | JS, React, CSS — explains the "why" | ![](https://www.youtube.com/@WebDevSimplified) |
| **Corey Schafer** | Intermediate/advanced Python | ![](https://www.youtube.com/@coreyms) |
| **Net Ninja** | Node.js, React, Vue — bite-sized | ![](https://www.youtube.com/@NetNinja) |
| **JavaScript Mastery** | Full project builds in React | ![](https://www.youtube.com/@javascriptmastery) |
| **Kevin Powell** | CSS master — best CSS YouTube channel | ![](https://www.youtube.com/@KevinPowell) |

---

## How to Know You're Ready for the Next Stage

✅ You've built and deployed at least one real project (not from a tutorial)
✅ You understand how APIs work and can fetch data from one
✅ You can use Git — commit, push, pull without looking up commands
✅ You've built something with React or a Python framework
✅ You can read documentation and figure out how to use a new library yourself
✅ You have a GitHub profile with code on it

**When all 6 are true → move to [[Master Stage]]**

---

## Related Notes
- [[Coding - Master Index]]
- [[Beginner Stage]]
- [[Master Stage]]
- [[JavaScript (JS)]]
- [[Python]]
- [[CSS]]
- [[SQL]]
- [[React]]
- [[Node.js]]
- [[Git and GitHub]]
- [[YouTube Channels for Coding]]
