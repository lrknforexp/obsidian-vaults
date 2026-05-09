# Node.js

> [!info] Quick Facts
> **Created:** 2009 by Ryan Dahl
> **Type:** JavaScript runtime environment (server-side JS)
> **Current Version:** Node.js 22 LTS (2025)
> **Used For:** Backend web servers, REST APIs, command-line tools, real-time apps
> **Prerequisite:** Must know [[JavaScript (JS)]] first
> **Difficulty:** ⭐⭐
> **Official Site:** https://nodejs.org/

---

**Node.js** lets you run [[JavaScript (JS)]] outside the browser — on a server. Before Node.js, JavaScript only ran in browsers. Now you can use the same language you use to build a website's frontend to also run its backend server, connect to databases, and handle HTTP requests.

---

## Core Concepts

### Basic HTTP Server
```javascript
const http = require("http");

const server = http.createServer((req, res) => {
  res.writeHead(200, { "Content-Type": "text/plain" });
  res.end("Hello from Node.js!");
});

server.listen(3000, () => {
  console.log("Server running at http://localhost:3000");
});
```

### Express.js (The Standard Web Framework)
```javascript
const express = require("express");
const app = express();

app.use(express.json()); // Parse JSON request bodies

// GET route
app.get("/", (req, res) => {
  res.send("Home page");
});

// GET with URL parameter
app.get("/users/:id", (req, res) => {
  const { id } = req.params;
  res.json({ userId: id, name: "Alex" });
});

// POST route
app.post("/users", (req, res) => {
  const { name, email } = req.body;
  // save to database...
  res.status(201).json({ message: "User created", name, email });
});

// PUT route
app.put("/users/:id", (req, res) => {
  res.json({ message: `User ${req.params.id} updated` });
});

// DELETE route
app.delete("/users/:id", (req, res) => {
  res.json({ message: `User ${req.params.id} deleted` });
});

app.listen(3000, () => console.log("API running on port 3000"));
```

### File System
```javascript
const fs = require("fs");

// Read a file
fs.readFile("data.txt", "utf8", (err, data) => {
  if (err) throw err;
  console.log(data);
});

// Write a file
fs.writeFile("output.txt", "Hello, file!", (err) => {
  if (err) throw err;
  console.log("File written!");
});

// Async versions (modern)
const { readFile, writeFile } = require("fs/promises");
const data = await readFile("data.txt", "utf8");
```

---

## npm — Node Package Manager

```bash
# Initialize a project
npm init -y

# Install a package (e.g. Express)
npm install express

# Install a dev dependency
npm install --save-dev nodemon

# Run a script from package.json
npm start
npm run dev

# Install all dependencies from package.json
npm install
```

---

## Setting Up a Node/Express Project

```bash
mkdir my-api
cd my-api
npm init -y
npm install express
npm install --save-dev nodemon
```

Add to `package.json`:
```json
"scripts": {
  "start": "node index.js",
  "dev": "nodemon index.js"
}
```

---

## Free Tutorials

- 🌐 **Node.js Official Docs:** https://nodejs.org/en/docs/
- 🌐 **Express.js Docs:** https://expressjs.com/

## YouTube Tutorials

| Video                                    | Link                                                                     |
| ---------------------------------------- | ------------------------------------------------------------------------ |
| Node.js Crash Course (Traversy Media)    | ![](https://www.youtube.com/watch?v=fBNz5xF-Kx4)                         |
| Express JS Crash Course (Traversy Media) | ![](https://www.youtube.com/watch?v=L72fhGm1tfE)                         |
| Node.js and Express — freeCodeCamp       | ![](https://www.youtube.com/watch?v=Oe421EPjeBE)                         |

---

## Related Notes
- [[Coding - Master Index]]
- [[JavaScript (JS)]]
- [[React]]
- [[SQL]]
- [[Amateur Stage]]
- [[Master Stage]]
