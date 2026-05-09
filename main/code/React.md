# React

> [!info] Quick Facts
> **Created:** 2013 by Facebook (Meta)
> **Type:** JavaScript library for building user interfaces
> **Current Version:** React 19 (2025)
> **Used For:** Frontend web apps, component-based UI
> **Prerequisite:** Must know [[JavaScript (JS)]] first
> **Difficulty:** ⭐⭐ — Easy to start, deep to master
> **Official Site:** https://react.dev/

---

**React** is the most popular frontend JavaScript library in the world. Instead of writing raw HTML that you update with JavaScript, you build **components** — reusable, self-contained pieces of UI. React handles updating the page efficiently when data changes.

---

## Core Concepts

### Components
```jsx
// A component is just a function that returns JSX (HTML-like syntax)
function Greeting({ name }) {
  return <h1>Hello, {name}!</h1>;
}

// Use it like an HTML tag
function App() {
  return (
    <div>
      <Greeting name="Alex" />
      <Greeting name="Sam" />
    </div>
  );
}
```

### State (useState)
```jsx
import { useState } from "react";

function Counter() {
  // [currentValue, functionToUpdateIt] = useState(initialValue)
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={() => setCount(count + 1)}>+1</button>
      <button onClick={() => setCount(count - 1)}>-1</button>
      <button onClick={() => setCount(0)}>Reset</button>
    </div>
  );
}
```

### Props (Passing Data to Components)
```jsx
// Parent passes data via attributes (props)
function App() {
  return <UserCard name="Alex" age={17} isAdmin={true} />;
}

// Child receives it as an object
function UserCard({ name, age, isAdmin }) {
  return (
    <div className="card">
      <h2>{name}</h2>
      <p>Age: {age}</p>
      {isAdmin && <span className="badge">Admin</span>}
    </div>
  );
}
```

### useEffect (Side Effects)
```jsx
import { useState, useEffect } from "react";

function UserList() {
  const [users, setUsers] = useState([]);
  const [loading, setLoading] = useState(true);

  // Runs after the component renders
  useEffect(() => {
    fetch("https://jsonplaceholder.typicode.com/users")
      .then(res => res.json())
      .then(data => {
        setUsers(data);
        setLoading(false);
      });
  }, []); // empty array = run once on mount

  if (loading) return <p>Loading...</p>;

  return (
    <ul>
      {users.map(user => (
        <li key={user.id}>{user.name} — {user.email}</li>
      ))}
    </ul>
  );
}
```

---

## Setting Up a React Project

```bash
# Create a new React app (Vite — modern, fast)
npm create vite@latest my-app -- --template react
cd my-app
npm install
npm run dev
```

---

## Free Tutorials

- 🌐 **Official React Docs (best):** https://react.dev/learn
- 🎓 **freeCodeCamp Front End Development Libraries:** https://www.freecodecamp.org/learn/front-end-development-libraries/

## YouTube Tutorials

| Video                                            | Link                                             |
| ------------------------------------------------ | ------------------------------------------------ |
| React Course for Beginners (freeCodeCamp, 12hrs) | ![](https://www.youtube.com/watch?v=bMknfKXIFA8) |
| React JS Crash Course (Traversy Media)           | ![](https://www.youtube.com/watch?v=w7ejDZ8SWv8) |
| React Tutorial (Web Dev Simplified)              | ![](https://www.youtube.com/watch?v=Rh3tobg7hEo) |
| React in 100 Seconds (Fireship)                  | ![](https://www.youtube.com/watch?v=Tn6-PIqc4UM) |

---

## Related Notes
- [[Coding - Master Index]]
- [[JavaScript (JS)]]
- [[TypeScript]]
- [[Node.js]]
- [[CSS]]
- [[Amateur Stage]]
- [[Master Stage]]
