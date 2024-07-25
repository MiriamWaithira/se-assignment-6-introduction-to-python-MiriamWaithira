[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15463505&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.


Python is an interpreted, object-oriented, high-level programming language with dynamic semantics.
Features:
i. Readability- it is easy to write and maintain as it emphasizes code blocks rather than curly braces
ii. Open-source- it is freely available and has large active community that contributes its development
iii. Compatibility- it can run on different operating systems with minimal modifications e.g. Windows, Linux, macOS.
iv. Interpreted- It is executed line by line allowing for rapid development and testing.
v. Extensive libraries- it has a vast ecosystem of libraries used for various tasks e.g. data science, machine learning, web development
vi. Object-Oriented- it supports object oriented programming that enables creation of modular and reusable code.

Use cases:
i. Data science and machine learning- it has libraries e.g. Numpy, pandas, matplotlib that are used for data manipulation and analysis
ii. Web development- It has frameworks like django and flask that simply creation of web applications from small-scale projects to complex platforms
iii. Automation- it's scripting capabilities allow for automating repetitive tasks eg. file management, data processing  and web scrapping
iv. Scientific computing- libraries such as SciPy and SymPy are used for complex calculations and simulations in fields like engineering and physics
v. Game development- libraries e.g. Pygame provide tools for creating 2D games, while frameworks like Unity support Python scripting for game logic.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.


Installation:
i. visit https://www.python.org/downloads/ to download the appropriate installer for your system.
ii. Navigate to the installer and double-click to start the installation process. Check the option written "Add Python to PATH" then click "Install Now".

Verification:
i. Open GitBash and type "python --version" and press enter.
ii. The installed  python version should be displayed.

Virtual Environment:
i. create and navigate to your project directory using "mkdir project" and "cd project"
ii. create the virtual environment using the command "python -m pip install virtualenv"
iii. name the virtual environment using the command "python -m virtualenv theproject".


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.


print("Hello, World!")
Syntax elements used:
i. print()- is a built-in python function used to display output on the console.
ii. Hello, World!- a string/ sequence of characters that will be displayed by the function print().
iii. ""- quotation marks enclose the string to be displayed.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.


Data types:
i. int- represents integers/ whole numbers
ii. float- represents numbers that have decimals e.g. 3.67
iii. str- represents sequence of characters e.g. "Hello, World!"
iv. bool- represents values that are either true of false
v. tuple- ordered list of items that cannot change e.g. coordinates = (36.7, 40.8)
vi. list- ordered list of items that can change e.g. apple, mango, banana.


x = 10  # int
y = 3.14  # float



name = "Alice"


fruits = ["apple", "mango", "banana"]  # list
coordinates = (36.7, 40.8)  # tuple



is_valid = True


print(type(x))
print(type(y))
print(type(name))
print(type(fruits))
print(type(coordinates))
print(type(is_valid))




5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.


Conditional statements allow your program to make decisions based on speceific conditions. Loops allow you to repeat a block of code multiple times.

Example of if-else statement:
balance = 500

if balance >= 500:
   print("Pocket money is enough.")
else:
   print("Balance is too low.")

Example of for loop:
fruits = ["apple", "banana", "mango"]

for fruit in fruits:
    print(fruit)


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.


Functions are reusable blocks of code that perform specific tasks. Useful because:
i. readability- they improve code organization and understanding
ii. testing- easier to test individual functions
iii. reusability- they avoid writing the same code multiple times
iv. modularity- they help to break down complex problems into smaller, manageable functions

Example:
def addition(num1, num2):

  sum = num1 + num2
  return sum


result = addition(3, 5)

print(result) 



7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.


Lists are ordered collection of items that can be changed and can contain duplicate elemets. Dictionaries are unordered collection of key-value pairs that are mutable and keys must be unique.

Example:

numbers = [1, 2, 3, 4, 5]


person = {'name': 'John', 'age': 30, 'city': 'Nairobi'}

print(numbers[2])
numbers.append(6)
numbers.remove(3)
print(numbers)


print(person['age'])
person['city'] = 'Kisumu'
person['occupation'] = 'Engineer'
print(person)

Output:
[Running] python -u "d:\TESTINGTU\lists.py"
3
[1, 2, 4, 5, 6]
30
{'name': 'John', 'age': 30, 'city': 'Kisumu', 'occupation': 'Engineer'}



8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.


Exception handling is a mechanism to manage errors that occur during program execution. It prevents your program from crashing and allows you to handle unexpected situations.
i. try- contains the code that might raise an execution
ii. except- defines the actions to be taken if an exception occurs
iii. finally- contains the code that always executes whether an exception occurs or not. It is used for cleanup operations like closing files or database connections

Example:
def divide(x, y):
  try:
    result = x / y
    print("Result:", result)
  except ZeroDivisionError:
    print("Error: Division by zero!")
  finally:
    print("This will always execute.")

divide(10, 2)
divide(10, 0)

Output:
i. divide(10, 2)
[Running] python -u "d:\TESTINGTU\exceptionhandling.py"
Result: 5.0
This will always execute.

ii. divide(10, 0)
[Running] python -u "d:\TESTINGTU\exceptionhandling.py"
Error: Division by zero!
This will always execute.


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.


A module is a python file that contains definitions and statements. it can define, functions, classes and variables.
A package is a directory that contains Python modules and possibly sub-packages.
Importing and using modules:
i. To import the entire module, use "import math"
ii. Use e.g. "math.sqrt(289)" to use the sqrt function to find the square root of 289.

Example:
import math

result = math.sqrt(289)
print(result)

Output:
[Running] python -u "d:\TESTINGTU\modules.py"
17.0


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.


Reading the contents of a file:
def read_file(filename):
  try:
    with open(filename, 'r') as file:
      contents = file.read()
      print(contents)
  except FileNotFoundError:
    print(f"File '{filename}' not found.")


read_file('contents.txt')
Output:
[Running] python -u "d:\TESTINGTU\reading.py"
This is how python can be used to read the contents of a file.

Writing strings:
def read_file(filename):
  try:
    with open(filename, 'r') as file:
      contents = file.read()
      print(contents)
  except FileNotFoundError:
    print(f"File '{filename}' not found.")

read_file('contents.txt')

Output:
This is line 1
This is line 2
This is line 3


REFERENCES


https://www.python.org/doc/essays/blurb/
https://www.geeksforgeeks.org/what-is-python/
https://www.youtube.com/watch?v=kqtD5dpn9C8



# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


