# Day 03 – Revisiting Python Fundamentals (CS50P)

**Date:** July 21, 2026

## 🎯 Objective

Today I officially began my Python revision using **CS50P (Introduction to Programming with Python)** as my primary learning resource.

Since I've been using Python since Class 12, this isn't about learning Python from scratch. Instead, my goal is to strengthen my fundamentals, replace beginner habits with professional coding practices, and build a solid foundation for AI Engineering.

---

## ✅ Completed Today

- Started the **Functions & Variables** lecture from CS50P.
- Took handwritten notes throughout the lecture instead of passively watching.
- Learned the basics of Python execution through the terminal.
- Understood functions, arguments, user input, return values, comments, print parameters, and format strings (f-strings).
- Finalized CS50P as my primary Python learning path.

---

# 📚 Concepts Learned

## 1. Running Python from the Terminal

Python programs can be executed directly from the terminal.

### Create a Python file

```bash
code hello.py
```

### Run the program

```bash
python hello.py
```

---

## 2. Functions

Functions perform specific tasks inside a program.

Example:

```python
print("Hello, World!")
```

Here,

- `print` → Function
- `"Hello, World!"` → Argument

---

## 3. Arguments

Arguments are inputs provided to functions that influence their behavior.

Example:

```python
print("Hello")
```

Here,

`"Hello"` is the argument passed to the `print()` function.

---

## 4. User Input

The `input()` function allows the user to interact with a program.

Example:

```python
name = input("What is your name? ")
```

One important thing I learned is:

> `input()` always returns a **string**, regardless of what the user types.

---

## 5. Return Values

Functions can return values that can later be stored or used.

Example:

```python
name = input("Name: ")
```

The value returned by `input()` is stored inside the variable `name`.

---

## 6. Printing Multiple Values

The `print()` function automatically separates multiple arguments with a space.

Example:

```python
name = "Owais"

print("Hello,", name)
```

Output

```
Hello, Owais
```

Instead of

```python
print("Hello," + name)
```

using multiple arguments is often cleaner.

---

## 7. Comments

Comments help explain code.

Python ignores them during execution.

Example:

```python
# Ask the user for their name

name = input("Name: ")
```

Comments improve readability and make future maintenance easier.

---

## 8. print() Parameters

The `print()` function has useful parameters.

### sep

Controls the separator between multiple objects.

```python
print("AI", "Engineer", sep="-")
```

Output

```
AI-Engineer
```

---

### end

Controls what is printed at the end of the line.

```python
print("Hello", end=" ")
print("Owais")
```

Output

```
Hello Owais
```

---

## 9. Format Strings (f-Strings)

Format strings provide a cleaner way to insert variables into text.

Example:

```python
name = "Owais"

print(f"Hello, {name}")
```

Output

```
Hello, Owais
```

I found this approach much more readable than string concatenation.

---

# 💻 Learning Evidence

Along with this journal, I also maintained handwritten notes while watching the lecture.

I want this repository to document my complete learning journey—not only polished solutions, but also the process of improving my understanding over time.

---

# 🧠 Biggest Takeaway

The biggest lesson from today's session wasn't Python syntax.

It was realizing that understanding the purpose behind each function and writing readable code is more valuable than simply memorizing syntax.

Even familiar concepts become more meaningful when revisited with the mindset of becoming a professional software engineer.

---

# 🚀 My Python Learning Strategy

After exploring multiple roadmaps, I decided to use **CS50P** as my primary resource for Python.

My workflow will be:

1. Learn a concept through CS50P.
2. Complete the associated problem set.
3. Fill knowledge gaps using official documentation or targeted resources.
4. Build a small project using what I learned.
5. Document my progress in this repository.

This approach emphasizes understanding over course completion.

---

# 📈 Areas to Improve

- Build cleaner coding habits.
- Write more readable code.
- Practice Python every day, even if only for a short period.
- Focus on consistency rather than speed.

---

# 🎯 Next Objective

- Complete the remaining portion of the **Functions & Variables** lecture.
- Solve the first CS50P problem set.
- Continue strengthening Python fundamentals before moving toward AI-focused libraries such as NumPy and Pandas.

## 🌱 Today's Reflection

### 💡 One thing I learned
Understanding that even simple Python concepts like `print()`, `input()`, and format strings have deeper functionality and are worth revisiting with a professional mindset.

---

### 🤔 One thing I found difficult
Maintaining focus throughout the long CS50P lecture. I realized that learning deeply requires patience, not just speed.

---

### 🚀 One thing I'll improve tomorrow
Complete the remaining portion of today's lecture and reinforce what I learned by solving the associated problem set and writing small practice programs.

---

### ⭐ One thing I'm proud of today
I started CS50P and documented my learning instead of simply watching the lecture passively. This journal is becoming evidence of my progress rather than just a collection of notes.
