# Python

> [!info] Quick Facts
> **Created:** 1991 by Guido van Rossum
> **Type:** High-level, interpreted, general-purpose programming language
> **Current Version:** Python 3.13 (2025)
> **Used For:** Web development, data science, AI/ML, automation, scripting, scientific computing
> **Difficulty:** ⭐ — Most beginner-friendly programming language
> **Official Site:** https://www.python.org/

---

**Python** is the **world's most popular programming language** as of 2025, holding over 23% of the TIOBE index. It was designed to be readable — Python code looks almost like plain English — making it the best first programming language for most people. It's also one of the most powerful, used everywhere from NASA to Netflix to Instagram.

---

## Why Learn Python?

- **Easiest language to start with** — minimal syntax, no semicolons, readable code
- **Incredibly versatile** — one language for web, AI, data, automation, games, and more
- **Massive ecosystem** — hundreds of thousands of libraries available via `pip`
- **Highest demand** in the job market for data science and AI roles
- **Huge community** — answers to almost every question are already on Stack Overflow

---

## Installing Python

1. Download from https://www.python.org/downloads/
2. During install, check **"Add Python to PATH"**
3. Open a terminal and type `python --version` to verify
4. Install **VS Code** as your editor (see [[Tools and Setup]])
5. Install the Python extension in VS Code

---

## Core Syntax

### Variables and Data Types
```python
# String
name = "Alex"

# Integer
age = 17

# Float
gpa = 3.8

# Boolean
is_student = True

# None (like null in other languages)
result = None

# Print
print(name, age, gpa)
print(f"Hello, {name}! You are {age} years old.")  # f-string
```

### Collections
```python
# List (ordered, changeable)
fruits = ["apple", "banana", "cherry"]
fruits.append("mango")
print(fruits[0])  # "apple"

# Dictionary (key-value pairs)
person = {"name": "Alex", "age": 17, "city": "New York"}
print(person["name"])  # "Alex"
person["email"] = "alex@email.com"  # add new key

# Tuple (ordered, unchangeable)
coordinates = (40.7128, -74.0060)

# Set (unordered, no duplicates)
unique_nums = {1, 2, 3, 3, 4}  # {1, 2, 3, 4}
```

### Conditionals
```python
score = 85

if score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
else:
    print("F")
```

### Loops
```python
# For loop
for i in range(5):       # 0, 1, 2, 3, 4
    print(i)

for fruit in fruits:
    print(fruit)

# While loop
count = 0
while count < 5:
    print(count)
    count += 1

# List comprehension (Python-specific shortcut)
squares = [x**2 for x in range(10)]  # [0, 1, 4, 9, 16, ...]
```

### Functions
```python
def greet(name, greeting="Hello"):
    return f"{greeting}, {name}!"

print(greet("Alex"))           # "Hello, Alex!"
print(greet("Sam", "Hey"))     # "Hey, Sam!"

# Lambda (anonymous function)
double = lambda x: x * 2
print(double(5))  # 10
```

### Classes and OOP
```python
class Dog:
    # Constructor
    def __init__(self, name, breed):
        self.name = name
        self.breed = breed

    def speak(self):
        return f"{self.name} says Woof!"

    def __str__(self):
        return f"Dog({self.name}, {self.breed})"

# Inheritance
class GuideDog(Dog):
    def __init__(self, name, breed, owner):
        super().__init__(name, breed)
        self.owner = owner

    def speak(self):
        return f"{self.name} says Woof! I guide {self.owner}."

rex = Dog("Rex", "German Shepherd")
print(rex.speak())
```

### Error Handling
```python
try:
    number = int(input("Enter a number: "))
    result = 100 / number
    print(result)
except ValueError:
    print("That's not a valid number!")
except ZeroDivisionError:
    print("Can't divide by zero!")
finally:
    print("This always runs.")
```

---

## Key Libraries (Install with `pip install <name>`)

| Library | Purpose | Command |
|---|---|---|
| **requests** | Make HTTP requests (call APIs) | `pip install requests` |
| **numpy** | Fast math and arrays | `pip install numpy` |
| **pandas** | Data tables / CSV analysis | `pip install pandas` |
| **matplotlib** | Charts and graphs | `pip install matplotlib` |
| **flask** | Lightweight web framework | `pip install flask` |
| **django** | Full-featured web framework | `pip install django` |
| **fastapi** | Modern API framework | `pip install fastapi` |
| **beautifulsoup4** | Web scraping | `pip install beautifulsoup4` |
| **selenium** | Browser automation | `pip install selenium` |
| **scikit-learn** | Machine learning | `pip install scikit-learn` |
| **sqlalchemy** | Database ORM | `pip install sqlalchemy` |

---

## Learning Path

| Level | Topics |
|---|---|
| **Beginner** | Variables, data types, loops, functions, basic I/O |
| **Amateur** | OOP, file handling, modules, pip libraries, error handling |
| **Master** | Async, decorators, metaclasses, type hints, performance, frameworks |

---

## Free Tutorials

- 🌐 **W3Schools Python:** https://www.w3schools.com/python/
- 🌐 **Real Python:** https://realpython.com/
- 🌐 **Automate the Boring Stuff (free book):** https://automatetheboringstuff.com/
- 🎓 **Harvard CS50P (free Python course):** https://cs50.harvard.edu/python/
- 🎓 **freeCodeCamp Python:** https://www.freecodecamp.org/learn/scientific-computing-with-python/

---

## YouTube Tutorials

| Video / Channel           | Description                                         | Link                                                                     |
| ------------------------- | --------------------------------------------------- | ------------------------------------------------------------------------ |
| **Programming with Mosh** | Python for Beginners (6hrs)                         | ![](https://www.youtube.com/watch?v=_uQrJ0TkZlc)                         |
| **freeCodeCamp**          | Python Full Course (4.5hrs)                         | ![](https://www.youtube.com/watch?v=rfscVS0vtbw)                         |
| **Tech with Tim**         | Python for Beginners                                | ![](https://www.youtube.com/watch?v=sxTmJE4k0ho)                         |
| **freeCodeCamp**          | Python for Everybody (Dr. Chuck, 14hrs)             | ![](https://www.youtube.com/watch?v=8DvywoWv6fI)                         |

---

## What You Can Build with Python

- **Web scraper** — automatically collect data from websites
- **Discord/Telegram bot** — automated chat bot
- **Data dashboard** — analyze CSV data and make charts
- **Web app** — full website with Django or Flask
- **REST API** — backend service with FastAPI
- **Machine learning model** — classify images, predict prices
- **Automation script** — rename files, send emails, fill forms automatically
- **Game** — 2D games with Pygame

---

## Related Notes
- [[Coding - Master Index]]
- [[Beginner Stage]]
- [[Amateur Stage]]
- [[Master Stage]]
- [[JavaScript (JS)]]
- [[SQL]]
- [[Git and GitHub]]
- [[YouTube Channels for Coding]]
- [[Free Resources and Websites]]
