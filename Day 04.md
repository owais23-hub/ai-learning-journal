# File: Day03.md

# 🚀 Day 03 – Functions, Scope & My First Python Project

**Date:** July 23, 2026

---

# 🎯 Objective

Today I continued my Python journey through **CS50P**, focusing on writing reusable code using functions, understanding variable scope and return values, working with string methods and numeric types, and finally applying everything I learned by building my first multi-function calculator.

This journey isn't about learning Python from scratch—I've been using Python since Class 12. Instead, my goal is to replace beginner habits with professional software engineering practices that will prepare me for AI Engineering.

---

# ✅ Completed Today

- Finished the Functions & Variables section covered today in CS50P.
- Learned how functions improve code organization.
- Understood local scope and why variables only exist where they are defined.
- Learned how `return` differs from `print()`.
- Explored string methods:
  - `strip()`
  - `capitalize()`
  - `title()`
  - `split()`
- Practiced working with:
  - `int()`
  - `float()`
  - `round()`
  - format strings (`f"{value:.2f}"`)
- Built my first function-based calculator project.

---

# 📚 Concepts Learned

## Functions

Functions allow code to be organized into reusable blocks.

Example

```python
def greet(name):
    return f"Hello, {name}"
```

Instead of repeating code multiple times, functions allow the same logic to be reused with different inputs.

---

## Parameters & Arguments

Parameters receive information inside a function.

```python
def greet(name):
    return f"Hello, {name}"
```

Here `name` is the parameter.

When calling

```python
greet("Owais")
```

"Owais" becomes the argument.

---

## Scope

A variable only exists inside the block where it was created.

Example

```python
def hello():
    name = "Owais"

print(name)
```

Output

```
NameError
```

because `name` only exists inside `hello()`.

---

## Return

Instead of printing inside a function, we can return a value back to the caller.

```python
def add(x, y):
    return x + y
```

This makes functions reusable and allows the main program to decide how the result should be displayed.

---

## String Methods

Today I explored several useful string methods.

```python
name = input("Name: ").strip().title()

first, last = name.split()
```

Methods learned:

- `strip()`
- `capitalize()`
- `title()`
- `split()`

---

## Numeric Types

```python
age = int(input("Age: "))
price = float(input("Price: "))
```

I also learned different ways to control decimal precision.

Using `round()`

```python
answer = round(result,2)
```

Using format strings

```python
print(f"{result:.2f}")
```

Dynamic precision

```python
print(f"{result:.{n}f}")
```

---

# 💻 Project Showcase

## 🧮 Smart Python Calculator

### Objective

Build a calculator that uses reusable functions instead of writing everything inside one large block of code.

### Features

- Addition
- Subtraction
- Multiplication
- Division
- Remainder
- User-defined decimal precision
- Function-based design
- Uses conditionals
- Uses formatted output

### Source Code

```python
def add(x, y):
    return x + y


def sub(x, y):
    return x - y


def multiply(x, y):
    return x * y


def divide(x, y):
    if y == 0:
        return "Cannot divide by zero."

    return x / y


def remainder(x, y):
    return x % y


def main():
    x = float(input("X: "))
    y = float(input("Y: "))
    n = int(input("Decimal Places: "))

    choice = int(input(
        """
1. Addition
2. Subtraction
3. Multiplication
4. Division
5. Remainder

Choice: """
    ))

    if choice == 1:
        result = add(x, y)
    elif choice == 2:
        result = sub(x, y)
    elif choice == 3:
        result = multiply(x, y)
    elif choice == 4:
        result = divide(x, y)
    elif choice == 5:
        result = remainder(x, y)
    else:
        print("Invalid Choice")
        return

    if isinstance(result, str):
        print(result)
    else:
        print(f"\nAnswer = {result:.{n}f}")


main()
```

---

# 🛠 Code Review

## ✅ What Went Well

- Broke the program into multiple reusable functions.
- Used `main()` to organize the execution flow.
- Accepted user input dynamically.
- Allowed users to choose decimal precision.
- Applied concepts from multiple lessons into one project.

---

## 🔄 Areas for Improvement

- Add exception handling using `try` and `except`.
- Replace the long `if-elif` chain with `match-case` (after learning it).
- Allow multiple calculations without restarting the program.
- Store previous calculations in a history list.
- Improve user interface with loops and menus.
- Continue separating logic from presentation using `return`.

---

# ⭐ Skills Gained

- Functions
- Parameters
- Arguments
- Variable Scope
- Return Values
- String Methods
- Integer & Float Conversion
- Output Formatting
- Problem Decomposition
- Program Organization

---

# 🌱 Today's Reflection

### 💡 One thing I learned

Functions make programs modular, reusable, and easier to maintain. I also understood why `return` is preferred over printing inside functions.

---

### 🤔 One thing I found difficult

Understanding when to use `print()`, `return`, `round()`, and formatted strings in the correct situations.

---

### 🚀 One thing I'll improve tomorrow

Practice writing more function-based programs and continue strengthening today's concepts through the CS50P problem set.

---

### ⭐ One thing I'm proud of today

I built my first complete function-based Python application by combining everything I learned into one project.

---

# 🧩 Connection to AI Engineering

Today's lesson reinforced that AI systems are built from many small, reusable components. Functions and clean program organization will become essential when I start building machine learning pipelines, training models, and developing AI applications.

---

# 🚀 Next Objective

- Complete the next CS50P lecture.
- Solve the associated problem set.
- Build another mini project using today's concepts.
- Continue documenting my progress as I work toward becoming an AI Engineer.

---

> **"Small improvements, repeated consistently, become expertise."**
