# Day 02 – Strengthening the Foundation

**Date:** July 13, 2026

## 🎯 Objective

Continue building a strong Python foundation by assessing my current problem-solving skills and identifying areas where I can improve my coding practices.

---

## ✅ Completed Today

* Solved three Python programming challenges without using AI assistance.
* Received a detailed code review focusing on software engineering practices rather than just correctness.
* Identified habits to improve before moving into more advanced Python and AI topics.
* Finalized my Python learning strategy using **CS50P** as my primary resource, supported by documentation, targeted videos, and mini projects.

---

## 💻 Programming Challenges

### Challenge 1 – Reverse a String

**My Solution**

```python
def reverse_string(input_string):#task 1 via loping
    r=input(str("Enter the string to be reversed:"))
    for i in range(len(r)-1, -1, -1):
        print(r[i], end="")


def reverse_using_slicing(input_string):# task 1 via slicing
    r=(input(str("Enter the string to be reversed by slicing")))
    print(r[::-1])
```

**Engineering Feedback**

* Logic was correct.
* Learned why functions should return values instead of printing them directly.
* Understood the importance of separating user input from processing logic.

---

### Challenge 2 – Word Frequency Counter

**My Solution**

```python

def Word_Frequency_Counter(input_string):#task 2  Word Frequency Counter
    r=(input(str("Enter the words to count their frequency:")))
    word_list = []
    w = r.split()
    word_list.append(w)
    fre={}
    for i in w:
        if i in fre:
            fre[i]+=1
        else:
            fre[i]=1
    for j in word_list and fre:
        print(j,":",i)    
```

**Engineering Feedback**

* Correct choice of using a dictionary.
* Identified unnecessary intermediate variables.
* Learned better ways to iterate through dictionaries.

---

### Challenge 3 – Remove Duplicates While Preserving Order

**My Solution**

```python
def remove_duplicates(input_list): #task 3  Remove Duplicates While Preserving Order
    r=(input(list("Enter the list to remove the Duplicates:")))
    unique_list=[]
    for i in r :
        if i not in unique_list:
            unique_list.append(i)
    print(unique_list)
```

**Engineering Feedback**

* Algorithm worked correctly.
* Need to improve how user input is converted into Python data structures.
* Will revisit this after learning more about input parsing and data handling.

---

## 🧠 Key Lesson

The most valuable lesson today wasn't about Python syntax—it was about software engineering.

A function should ideally have a single responsibility: receive data, process it, and return a result. Mixing user input, business logic, and output makes code harder to reuse, test, and maintain.

This shifted my perspective from simply writing working programs to writing cleaner, more maintainable code, and the more use of functions the faster is the execution time

---

## 📚 Current Learning Path

To strengthen my Python fundamentals, I've decided to use **CS50P** as my primary learning resource.

My workflow will be:

1. Learn a concept through CS50P.
2. Complete the associated problem sets.
3. Fill any knowledge gaps using official documentation or targeted resources.
4. Build a small project to apply what I've learned.
5. Document my progress and reflections in this repository.

My goal is not to relearn Python from scratch but to refine my existing knowledge and adopt professional engineering practices.

---

## 📈 Areas to Improve

* Write cleaner, reusable functions.
* Separate input, processing, and output.
* Use more Pythonic approaches where appropriate.
* Improve code readability and organization.
* Build habits that scale to larger software projects.

---

## 🎯 Next Objective

Continue through the Functions & Variables section of CS50P and apply the concepts by improving today's programs instead of simply writing new ones.
on programmer.
