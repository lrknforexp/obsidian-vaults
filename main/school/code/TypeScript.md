# TypeScript

> [!info] Quick Facts
> **Created:** 2012 by Microsoft
> **Type:** Superset of [[JavaScript (JS)]] — compiles to plain JS
> **Current Version:** TypeScript 5.x (2025)
> **Used For:** Everything JS is used for, but safer and more scalable
> **Difficulty:** ⭐⭐ — Learn JS first, then TypeScript is quick to pick up
> **Official Site:** https://www.typescriptlang.org/

---

**TypeScript** is JavaScript with **static types**. Every valid JavaScript program is valid TypeScript — TypeScript just adds an optional type system on top. It catches bugs while you're writing code rather than when your users encounter them. Almost every serious modern JavaScript project uses TypeScript.

---

## Why TypeScript?

```javascript
// JavaScript: No error until runtime
function getLength(str) {
  return str.length;
}
getLength(42);  // Crashes! Numbers don't have .length
```

```typescript
// TypeScript: Error immediately in your editor
function getLength(str: string): number {
  return str.length;
}
getLength(42);  // ERROR: Argument of type 'number' is not assignable to 'string'
```

---

## Basic Types

```typescript
// Primitive types
let name: string = "Alex";
let age: number = 17;
let isStudent: boolean = true;
let nothing: null = null;
let notDefined: undefined = undefined;

// Arrays
let scores: number[] = [95, 87, 92];
let names: string[] = ["Alex", "Sam"];
let mixed: (string | number)[] = ["hello", 42];

// Any (escape hatch — avoid using this)
let anything: any = "can be anything";

// Unknown (safer than any)
let unknown: unknown = someExternalData;
```

## Interfaces and Types

```typescript
// Interface — define the shape of an object
interface User {
  id: number;
  name: string;
  email: string;
  age?: number;         // optional property
  readonly createdAt: Date;  // can't be changed after creation
}

// Using it
const user: User = {
  id: 1,
  name: "Alex",
  email: "alex@email.com",
  createdAt: new Date()
};

// Type alias
type ID = string | number;
type Status = "active" | "inactive" | "pending";

let status: Status = "active";
// status = "banana"  // ERROR!
```

## Functions with Types

```typescript
// Parameter and return types
function add(a: number, b: number): number {
  return a + b;
}

// Optional parameter
function greet(name: string, greeting?: string): string {
  return `${greeting ?? "Hello"}, ${name}!`;
}

// Arrow function with types
const multiply = (a: number, b: number): number => a * b;

// Async function
async function fetchUser(id: number): Promise<User> {
  const response = await fetch(`/api/users/${id}`);
  return response.json();
}
```

## Generics

```typescript
// Reusable functions that work with any type
function identity<T>(value: T): T {
  return value;
}

identity<string>("hello");  // returns string
identity<number>(42);       // returns number

// Generic interface
interface ApiResponse<T> {
  data: T;
  status: number;
  message: string;
}

const userResponse: ApiResponse<User> = {
  data: { id: 1, name: "Alex", email: "alex@email.com", createdAt: new Date() },
  status: 200,
  message: "OK"
};
```

---

## Installing TypeScript

```bash
# Install globally
npm install -g typescript

# Or in a project
npm install --save-dev typescript

# Compile a TypeScript file to JavaScript
tsc myfile.ts

# Initialize a project config
tsc --init
```

---

## Free Tutorials

- 🌐 **TypeScript Official Docs:** https://www.typescriptlang.org/docs/
- 🌐 **TypeScript Handbook:** https://www.typescriptlang.org/docs/handbook/intro.html
- 🎓 **The Odin Project TypeScript:** https://www.theodinproject.com/

## YouTube Tutorials

| Video | Link |
|---|---|
| TypeScript Crash Course (Traversy Media) | ![](https://www.youtube.com/watch?v=BCg4U1FzODs) |
| TypeScript Full Course (freeCodeCamp) | ![](https://www.youtube.com/watch?v=30LWjhZzg50) |
| TypeScript for Beginners (Programming with Mosh) | ![](https://www.youtube.com/watch?v=d56mG7DezGs) |
| TypeScript in 100 Seconds (Fireship) | ![](https://www.youtube.com/watch?v=zQnBQ4tB3ZA) |

---

## Related Notes
- [[Coding - Master Index]]
- [[JavaScript (JS)]]
- [[React]]
- [[Node.js]]
- [[Master Stage]]
