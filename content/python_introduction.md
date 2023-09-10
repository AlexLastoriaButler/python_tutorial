---
jupyter:
  kernelspec:
    display_name: Python 3 (ipykernel)
    language: python
    name: python3
  language_info:
    codemirror_mode:
      name: ipython
      version: 3
    file_extension: .py
    mimetype: text/x-python
    name: python
    nbconvert_exporter: python
    pygments_lexer: ipython3
    version: 3.11.5
  nbformat: 4
  nbformat_minor: 5
---

::: {#9e5ce2e6-7614-403a-b1ba-721b0bef0a9e .cell .markdown editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
# Introduction

## 1.1 What is Python? {#11-what-is-python}

Python is a high-level, interpreted programming language known for its
readability and simplicity. It\'s widely used in data analysis, web
development, artificial intelligence, and more.
:::

::: {#e70bec40-e0d7-426d-a8fd-8342ad35d11e .cell .markdown editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
## 1.2 Installing Python {#12-installing-python}

Before we begin, make sure you have Python installed on your computer.
You can download it from Python\'s official website.
:::

::: {#b7d79c52-599c-448e-b1ea-41acc47719c5 .cell .markdown editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
## 1.3 Your First Python Program {#13-your-first-python-program}

Open a text editor (like Notepad) and create a new file with the
extension .py. Let\'s write your first Python program:
:::

::: {#f2d71d14-efb1-4b5a-9cba-7f7d0e7ec8bb .cell .code editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
``` python
# This is a comment 
print("Hello, world!")
```
:::

::: {#bb521a86-7d75-4102-974d-c06e95d59502 .cell .markdown editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
Save the file and run it using the command python filename.py in your
terminal.
:::

::: {#f04bb971-78ba-4690-a615-7fd97a1a137e .cell .markdown editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
## 1.4 Variables and Data Types {#14-variables-and-data-types}

In Python, you can store data in variables. Python supports various data
types:

-   int: Integer
-   float: Floating-point number
-   str: String
-   bool: Boolean (True or False)
:::

::: {#be58a2ea-c70a-4d37-bf63-5b768b1e4324 .cell .code editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
``` python
age = 25 
name = "Alice" 
is_student = True
score = "86"
# Note, score will be treated as a character variable unless converted
```
:::

::: {#d3881079-e579-4ad0-83b4-6d04e249586a .cell .markdown editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
## 1.5 Basic Operations {#15-basic-operations}
:::

::: {#fea0fb26-d3a1-41f3-b565-995a8ba98666 .cell .code editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
``` python
# Arithmetic operations 
result = 5 + 3 
difference = 10 - 2 
product = 4 * 7 
quotient = 20 / 5 

# Modulus (remainder) 
remainder = 11 % 3 

# Exponentiation 
power = 2 ** 3
```
:::

::: {#bf735d1d-9a0c-4da2-83a2-72b6186f3c24 .cell .markdown editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
## 1.6 Conditional Statements (IF THEN ELSE) {#16-conditional-statements-if-then-else}

Use if, elif, and else to make decisions in your code:
:::

::: {#421c6cad-e33e-4c0c-b449-94a237af290a .cell .code editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
``` python
score = 87

if age < 80: 
    print("Below required score") 
elif age == 80: 
    print("Meets requirement") 
else: 
    print("Exceeds required score")
```
:::

::: {#ed49d060-521b-4af8-be34-8b47a67d3fa5 .cell .markdown editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
Note the indenting after each condition, this is a PEP-81 standard. Most
IDE's will warn you if indentation is used incorrectly or
inconsistently.
:::

::: {#e94a4916-bd58-48ed-9eb1-546f5ef4ddbf .cell .markdown editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
## 1.7 Loops {#17-loops}
:::

::: {#40e7f4f0-aaa4-4510-a116-e3c331cd516c .cell .code editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
``` python
# For loop 
for i in range(5): 
    print(i) 

# For loop using a list
list = ["a", "b", "c"]
for i in list: 
    print(i) 

# While loop 
count = 0 
while count < 5: 
    print(count) 
    count += 1
```
:::

::: {#7e1f6816-bebc-4c4a-bfed-7f4a5bad4967 .cell .markdown editable="true" slideshow="{\"slide_type\":\"\"}" tags="[]"}
## Exercises

-   Write a Python program that calculates the area of a rectangle with
    a length of 6 and width of 4.5
-   Create a program that checks if a number is even or odd
-   Write a loop that prints the first 10 even numbers (starting from 2)
-   Develop a simple calculator program that can add, subtract,
    multiply, and divide two numbers based on user input
:::
