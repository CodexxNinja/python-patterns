# Python - Complete Introduction and Pattern Programs

## What is Python?

Python is a **high-level, interpreted, object-oriented, and general-purpose programming language**. It was created by **Guido van Rossum** and first released in **1991**. Python emphasizes **code readability** with a simple and easy-to-understand syntax, making it one of the most popular programming languages in the world.

Python is widely used in:

- Web Development
- Data Science
- Artificial Intelligence (AI)
- Machine Learning (ML)
- Automation and Scripting
- Cybersecurity
- Cloud Computing
- Desktop Application Development
- Game Development
- Internet of Things (IoT)

---

# History of Python

- **1989:** Guido van Rossum started working on Python.
- **1991:** Python 0.9.0 was released.
- **2000:** Python 2.0 introduced new features.
- **2008:** Python 3.0 was released with major improvements.
- **Today:** Python 3.x is actively maintained and recommended.

---

# Features of Python

## 1. Easy to Learn

Python has simple syntax that resembles English, making it beginner-friendly.

Example:

```python
print("Hello, World!")
```

---

## 2. Interpreted Language

Python code is executed line by line without requiring compilation.

Advantages:
- Faster development
- Easier debugging
- Platform independence

---

## 3. High-Level Language

Python handles memory management automatically.

Example:

```python
name = "Alice"
age = 20
```

---

## 4. Object-Oriented

Python supports:

- Classes
- Objects
- Inheritance
- Polymorphism
- Encapsulation
- Abstraction

Example:

```python
class Student:
    def __init__(self, name):
        self.name = name

student = Student("John")
print(student.name)
```

---

## 5. Cross-Platform

Python runs on:

- Windows
- Linux
- macOS

The same code works with little or no modification.

---

## 6. Open Source

Python is free to use and has a large community contributing libraries and tools.

---

## 7. Large Standard Library

Python includes built-in modules such as:

- math
- random
- datetime
- os
- sys
- json
- collections

Example:

```python
import math

print(math.sqrt(25))
```

---

# Applications of Python

## Web Development

Popular frameworks:

- Django
- Flask
- FastAPI

Example:

```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "Welcome"

app.run()
```

---

## Data Science

Libraries:

- NumPy
- Pandas
- Matplotlib
- Seaborn

Example:

```python
import pandas as pd

data = pd.read_csv("data.csv")
print(data.head())
```

---

## Machine Learning

Libraries:

- Scikit-learn
- TensorFlow
- PyTorch

Example:

```python
from sklearn.linear_model import LinearRegression
```

---

## Artificial Intelligence

Python is widely used for:

- Chatbots
- Computer Vision
- Speech Recognition
- Recommendation Systems

Libraries:

- OpenCV
- TensorFlow
- Keras
- Transformers

---

## Automation

Example:

```python
import os

os.mkdir("NewFolder")
```

---

## Game Development

Library:

- Pygame

---

## Cybersecurity

Used for:

- Ethical hacking
- Network scanning
- Security testing

Libraries:

- Scapy
- Requests

---

# Advantages of Python

- Easy syntax
- Large community
- Huge library support
- Fast development
- Portable
- Open source
- Object-oriented
- Dynamic typing
- Excellent documentation

---

# Disadvantages of Python

- Slower than C/C++
- Higher memory usage
- Not ideal for mobile apps
- Runtime errors due to dynamic typing

---

# Python Installation

## Step 1

Download Python from:

https://python.org

---

## Step 2

Run the installer.

✔ Check:

```
Add Python to PATH
```

---

## Step 3

Verify installation

```bash
python --version
```

or

```bash
python3 --version
```

---

# First Python Program

```python
print("Hello, World!")
```

Output

```
Hello, World!
```

---

# Python Syntax Basics

## Variables

```python
name = "Alice"
age = 25
height = 5.7
```

---

## Data Types

```python
int
float
str
bool
list
tuple
set
dict
```

Example:

```python
x = 10
y = 3.14
name = "Python"
status = True
```

---

## Input

```python
name = input("Enter your name: ")
print(name)
```

---

## Output

```python
print("Hello")
```

---

# Control Statements

## If Statement

```python
age = 20

if age >= 18:
    print("Adult")
```

---

## If Else

```python
age = 15

if age >= 18:
    print("Adult")
else:
    print("Minor")
```

---

## Loops

### For Loop

```python
for i in range(5):
    print(i)
```

### While Loop

```python
count = 0

while count < 5:
    print(count)
    count += 1
```

---

# Functions

```python
def greet(name):
    return "Hello " + name

print(greet("John"))
```

---

# Lists

```python
fruits = ["Apple", "Banana", "Mango"]

print(fruits[0])
```

---

# Dictionaries

```python
student = {
    "name": "John",
    "age": 20
}

print(student["name"])
```

---

# Exception Handling

```python
try:
    x = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
```

---

# File Handling

```python
with open("file.txt", "w") as file:
    file.write("Hello Python")
```

---

# Python Project Structure (Starter Pattern)

A common Python project layout:

```
project_name/
│
├── README.md
├── requirements.txt
├── .gitignore
├── main.py
├── config.py
├── app/
│   ├── __init__.py
│   ├── models.py
│   ├── views.py
│   └── utils.py
├── tests/
│   └── test_main.py
└── data/
```

---

# Python Starter Patterns

## 1. Basic Script Pattern

```python
def main():
    print("Hello Python")

if __name__ == "__main__":
    main()
```

This is the recommended pattern for standalone Python scripts.

### Why use it?

- Makes code reusable as a module.
- Prevents code from running when imported.
- Keeps the program organized.

---

## 2. Object-Oriented Pattern

```python
class Person:
    def __init__(self, name):
        self.name = name

    def greet(self):
        print(f"Hello, {self.name}")

person = Person("Alice")
person.greet()
```

Suitable for medium to large applications.

---

## 3. Package-Based Pattern

```
my_project/
├── package/
│   ├── __init__.py
│   ├── module1.py
│   └── module2.py
├── main.py
└── README.md
```

Useful for organizing reusable code.

---

## 4. Virtual Environment Pattern

```bash
python -m venv venv
```

Activate the environment:

**Windows**

```bash
venv\Scripts\activate
```

**Linux/macOS**

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 5. Web Application Pattern (Flask)

```
my_flask_app/
├── app.py
├── templates/
├── static/
├── requirements.txt
└── README.md
```

---

## 6. Data Science Pattern

```
project/
├── data/
├── notebooks/
├── models/
├── scripts/
├── requirements.txt
└── README.md
```

---

# Best Practices

- Use meaningful variable names.
- Follow PEP 8 style guidelines.
- Write reusable functions.
- Use virtual environments.
- Add comments and documentation.
- Handle exceptions properly.
- Write unit tests.
- Keep project structure organized.

---

# Popular Python Libraries

| Library | Purpose |
|----------|---------|
| NumPy | Numerical computing |
| Pandas | Data analysis |
| Matplotlib | Visualization |
| Seaborn | Statistical plots |
| Scikit-learn | Machine learning |
| TensorFlow | Deep learning |
| PyTorch | AI and ML |
| Flask | Web development |
| Django | Full-stack web framework |
| FastAPI | High-performance APIs |
| OpenCV | Computer vision |
| Requests | HTTP requests |
| BeautifulSoup | Web scraping |

---

# Conclusion

Python is one of the most versatile and beginner-friendly programming languages available today. Its simple syntax, extensive ecosystem of libraries, and strong community support make it an excellent choice for tasks ranging from automation and web development to artificial intelligence and data science. By learning Python's fundamentals, adopting standard project structures (starter patterns), and following best practices, developers can build clean, scalable, and maintainable applications.
