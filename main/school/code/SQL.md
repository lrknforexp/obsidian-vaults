# SQL

> [!info] Quick Facts
> **Full Name:** Structured Query Language
> **Pronunciation:** "sequel" or "S-Q-L"
> **Created:** 1974 at IBM
> **Type:** Query language for relational databases
> **Used For:** Reading, writing, and managing data in databases
> **Difficulty:** ⭐⭐ — Logical and readable once you get the pattern
> **Official Standard:** ISO/IEC 9075

---

**SQL** is how you talk to databases. Every app that stores data — social media, e-commerce, banking, games — uses a database behind the scenes, and SQL is the language used to read and write that data. It's one of the most consistently in-demand skills in tech.

---

## Popular SQL Databases

| Database | Best For | Notes |
|---|---|---|
| **SQLite** | Learning, small apps | File-based, no server needed |
| **PostgreSQL** | Production apps | Powerful, open-source, professional standard |
| **MySQL** | Web apps | Most common with PHP/WordPress |
| **Microsoft SQL Server** | Enterprise | Windows environments |

---

## Core SQL Commands

### SELECT — Read Data
```sql
-- Get all columns from a table
SELECT * FROM users;

-- Get specific columns
SELECT name, email, age FROM users;

-- Filter rows
SELECT * FROM users WHERE age > 18;
SELECT * FROM users WHERE city = 'New York';

-- Sort results
SELECT * FROM users ORDER BY age DESC;

-- Limit results
SELECT * FROM users LIMIT 10;

-- Combined
SELECT name, email FROM users
WHERE age >= 18
ORDER BY name ASC
LIMIT 20;
```

### INSERT — Add Data
```sql
INSERT INTO users (name, email, age)
VALUES ('Alex', 'alex@email.com', 17);

-- Multiple rows at once
INSERT INTO users (name, age) VALUES
  ('Sam', 19),
  ('Jordan', 22),
  ('Taylor', 16);
```

### UPDATE — Modify Data
```sql
-- Update specific rows (ALWAYS use WHERE or you change everything)
UPDATE users
SET age = 18
WHERE name = 'Alex';

-- Update multiple columns
UPDATE users
SET email = 'newemail@gmail.com', city = 'Boston'
WHERE id = 42;
```

### DELETE — Remove Data
```sql
-- Delete specific rows (ALWAYS use WHERE)
DELETE FROM users WHERE id = 42;
DELETE FROM users WHERE age < 13;
```

### CREATE TABLE — Define Structure
```sql
CREATE TABLE users (
  id        INTEGER PRIMARY KEY AUTOINCREMENT,
  name      TEXT NOT NULL,
  email     TEXT UNIQUE NOT NULL,
  age       INTEGER,
  city      TEXT DEFAULT 'Unknown',
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

### JOIN — Combine Tables
```sql
-- Tables: users(id, name) and orders(id, user_id, product, price)

-- INNER JOIN — only matching rows
SELECT users.name, orders.product, orders.price
FROM orders
INNER JOIN users ON orders.user_id = users.id;

-- LEFT JOIN — all users, even with no orders
SELECT users.name, orders.product
FROM users
LEFT JOIN orders ON orders.user_id = users.id;
```

### Aggregate Functions
```sql
SELECT COUNT(*) FROM users;                    -- total rows
SELECT AVG(age) FROM users;                    -- average age
SELECT MAX(price) FROM products;               -- highest price
SELECT MIN(price) FROM products;               -- lowest price
SELECT SUM(price) FROM orders WHERE user_id=1; -- total spent

-- GROUP BY
SELECT city, COUNT(*) as user_count
FROM users
GROUP BY city
ORDER BY user_count DESC;
```

---

## Free Tutorials

- 🌐 **W3Schools SQL:** https://www.w3schools.com/sql/
- 🎓 **SQLZoo (interactive):** https://sqlzoo.net/
- 🎓 **freeCodeCamp Relational Database:** https://www.freecodecamp.org/learn/relational-database/

## YouTube Tutorials

| Video | Link |
|---|---|
| SQL Full Course (freeCodeCamp, 4hrs) | ![](https://www.youtube.com/watch?v=HXV3zeQKqGY) |
| SQL Crash Course (Traversy Media) | ![](https://www.youtube.com/watch?v=9ylj9NR0Lcg) |
| SQL for Beginners (Programming with Mosh) | ![](https://www.youtube.com/watch?v=7S_tz1z_5bA) |

---

## Related Notes
- [[Coding - Master Index]]
- [[Python]]
- [[Node.js]]
- [[Amateur Stage]]
- [[Master Stage]]
