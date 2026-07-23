# 🚀 Day 04 – From Writing Code to Designing Programs

**Date:** July 23, 2026

---

# 🎯 Mission

Today's goal was to move beyond simply writing Python statements and begin thinking like a software engineer. I focused on understanding how functions, scope, return values, and data formatting work together to build structured, reusable programs.

Instead of stopping at theory, I applied everything by building my first modular Python calculator.

---

# ✅ Mission Accomplished

- Continued CS50P (Functions & Variables).
- Learned how to create custom functions using `def`.
- Understood the difference between **parameters** and **arguments**.
- Learned how **scope** controls where variables exist.
- Understood the purpose of the `return` keyword.
- Practiced converting user input using `int()` and `float()`.
- Learned to control floating-point precision using `round()` and formatted strings.
- Explored useful string methods:
  - `strip()`
  - `capitalize()`
  - `title()`
  - `split()`
- Built my first complete function-based calculator.

---

# 📚 Engineering Concepts

## Functions

Functions allow code to be written once and reused many times.

Instead of repeating the same logic, we define a function and call it whenever needed.

```python
def greet(name):
    return f"Hello, {name}"
```

---

## Parameters vs Arguments

```python
def greet(name):
    return f"Hello, {name}"
```

`name` is the **parameter**.

```python
greet("Owais")
```

`"Owais"` is the **argument**.

---

## Scope

One of the biggest concepts I learned today was **scope**.

A variable only exists inside the block or function where it was created.

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

Another important concept was **return**.

Instead of displaying the answer immediately, a function can send it back to another part of the program.

```python
def add(x, y):
    return x + y
```

This makes functions reusable and allows the caller to decide how the result should be used.

---

## Numeric Formatting

Today I explored two ways to control decimal precision.

Using `round()`

```python
result = round(answer, 2)
```

Using formatted strings

```python
print(f"{answer:.2f}")
```

Dynamic formatting

```python
print(f"{answer:.{n}f}")
```

---

## String Methods

Useful methods learned today:

```python
name = input("Name: ").strip().title()
```

Methods explored

- `strip()`
- `capitalize()`
- `title()`
- `split()`

These methods make user input cleaner and easier to process.

---

# 💻 Engineering Log — Project 001

# 🧮 Modular Python Calculator

## Objective

Build a calculator that applies everything learned so far by separating each mathematical operation into its own function.

---

## Skills Used

- Functions
- Parameters
- Arguments
- Scope
- Return Values
- `int()`
- `float()`
- Formatted Strings
- Conditionals
- User Input

---

## Source Code

```python
# Mathematical Operations

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


# Main Program

def main():
    x = float(input("X? "))
    y = float(input("Y? "))
    n = int(input("Number of digits after decimal: "))

    choice = int(input(
        """
1. Addition
2. Subtraction
3. Multiplication
4. Division
5. Remainder

Choose an operation: """
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

# 🛠 Engineering Decisions

While building this calculator, I made an important design improvement.

Initially, each function calculated **and printed** its own result.

After learning about `return`, I refactored the program so that each function is responsible only for performing its calculation.

The `main()` function now handles displaying the output.

This separation of logic and presentation makes the code cleaner, more reusable, and easier to maintain.

---

# 🐛 Mistakes & Improvements

### Mistakes I Found

- Initially named the remainder function `reminder()` instead of `remainder()`.
- Printed results directly inside functions instead of returning them.
- Did not initially handle division by zero.

### Improvements Made

- Switched to `return` in every function.
- Added protection against division by zero.
- Moved formatting to the main program.
- Improved function naming for better readability.

---

# ⭐ Skills Earned Today

- Writing reusable functions
- Passing parameters
- Understanding variable scope
- Returning values from functions
- Formatting numerical output
- Organizing larger programs
- Separating logic from presentation

---

# 🧠 Biggest Engineering Insight

Today's biggest lesson wasn't learning a new Python keyword.

It was understanding that **good software design is about responsibility**.

Each function should have one clear job.

When every part of a program has a single responsibility, the entire program becomes easier to understand, test, debug, and improve.

This idea will become increasingly important as I begin building larger AI and Machine Learning systems.

---

# 🌱 Today's Reflection

### 💡 One thing I learned

Returning values from functions makes programs significantly more flexible than printing directly inside them.

---

### 🤔 One thing I found difficult

Understanding where data should be processed versus where it should be displayed.

---

### 🚀 One thing I'll improve tomorrow

I'll continue practicing function-based programming by solving the CS50P problem set and writing programs without relying on my notes.

---

### ⭐ One thing I'm proud of today

Today I built my first structured Python application instead of a single script. More importantly, I improved it after learning better engineering practices rather than settling for a working solution.

---

# 🧩 Connection to AI Engineering

Modern AI applications are built from many small, reusable components.

Today's lesson on functions and separation of responsibilities mirrors how real AI systems are developed. Data loading, preprocessing, model training, evaluation, and deployment are all separated into independent modules.

Learning to write clean, modular Python code today lays the foundation for building production-ready AI systems in the future.

---

> **"Every expert once wrote code they would never deploy. Improvement begins the moment you start refactoring your own work."
