# Introduction

## 1.1 What is Python?
Python is a high-level, interpreted programming language known for its readability and simplicity. It's widely used in data analysis, web development, artificial intelligence, and more.

## 1.2 Installing Python
Before we begin, make sure you have Python installed on your computer. You can download it from Python's official website.

## 1.3 Your First Python Program
Open a text editor (like Notepad) and create a new file with the extension .py. Let's write your first Python program:

``` py
# This is a comment 
print("Hello, world!")
Save the file and run it using the command python filename.py in your terminal.
```

## 1.4 Variables and Data Types
In Python, you can store data in variables. Python supports various data types:
int: Integer
float: Floating-point number
str: String
bool: Boolean (True or False)
``` py
age = 25 
name = "Alice" 
is_student = True
score = "86"
# Note, score will be treated as a character variable unless converted
```

## 1.5 Basic Operations
``` py
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
## 1.6 Conditional Statements (IF THEN ELSE)
Use if, elif, and else to make decisions in your code:
``` py
score = 87

if score < 80: 
    print("Below required score") 
elif score == 80: 
    print("Meets requirement") 
else: 
    print("Exceeds required score")
```
Note the indenting after each condition, this is a PEP-81 standard. Most IDE’s will warn you if indentation is used incorrectly or inconsistently.

## 1.7 Loops
``` py
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
## Exercises
Write a Python program that calculates the area of a rectangle with a length of 6 and width of 4.5
Create a program that checks if a number is even or odd
Write a loop that prints the first 10 even numbers (starting from 2)
Develop a simple calculator program that can add, subtract, multiply, and divide two numbers based on user input
Click to add a cell.
