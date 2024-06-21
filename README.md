[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15306845&assignment_repo_type=AssignmentRepo)

# SE-Assignment-6

Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

Questions:

1. Python Basics:

   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
     Answer
     Python is a high-level interprated programming language.
     key features:
   - readability and simplicity: python sysntax is easy to read.
   - interprated language: python code executes line by line for easy debugging
   - extensive standard library: python has libraries that support many programmin tasks
   - Object oriented programming: python supports creation of reusable and modular code.
   - Cross platform: python can run in many devices with different operating systems
     python can be used in web development, data analysis and scientific computing, machine learning and artificial intelligence, automation and scripting, software development and more.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
     Answer

Windows:

Download the installer from python.org.
Run the installer, check "Add Python to PATH", and click "Install Now".
Verify installation by running python --version in Command Prompt.
Create a virtual environment: python -m venv myenv.
Activate it: myenv\Scripts\activate.

3. Python Syntax and Semantics:

   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
     Answer
     print("Hello, World!")
     print(): A function that outputs text to the console.
     "Hello, World!": A string enclosed in quotes.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
     Answer
     Basic data types:

integer: Integer numbers (e.g., 10)
float: Floating-point numbers (e.g., 10.5)
string: Strings (e.g., "Hello")
boolean: Boolean values (True or False)
list: Ordered sequences (e.g., [1, 2, 3])
dictonary: Key-value pairs (e.g., {"a": 1, "b": 2})
bellow is the sample code

age = 20 # integer
height = 5.9 # float
name = "Alan" # string
is_student = True # boolean
numbers = [1, 2, 3] # list
person = {"name": "Alan", "age": 20} # dictonary

print(age, height, name, is_student, numbers, person)

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
     Answer
     They allow you to make decisions based on the values of variables or the result of comparisons
     if else example:
     age = 20
     if age >= 18:
     print("Adult")
     else:
     print("Minor")

for loop exapmle
for i in range(5):
print(i)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
     Answer
     A function is a named section of code that performs a specific task.
     they are useful because they save alot of time when coding, they also provide reusable code.
     example
     def add(a, b):
     return a + b

result = add(3, 5)
print(result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
     Answer
     Lists are ordered collections accessed by index.
     Dictionaries are unordered collections accessed by keys.
     list example
     numbers = [1, 2, 3]
     numbers.append(4)
     print(numbers)

dictionary example
person = {"name": "Alice", "age": 25}
person["age"] = 26
print(person)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
     Answer
     Exception handling manages erros in your code

example code
try:
x = int(input("Enter a number: "))
print(10 / x)
except ValueError:
print("Invalid number")
except ZeroDivisionError:
print("Cannot divide by zero")
finally:
print("Finished")

9. Modules and Packages:

   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
     Answer
     Modules are files containing Python code. Packages are directories containing multiple modules.
     example code:
     import math

print(math.sqrt(16))

10. File I/O: - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    Answer
    To read from a file in Python

Open the file: Use the open() function with the file path and mode 'r' for reading
Read from the file: Use methods like read(), readline(), or readlines() to retrieve the content.
Close the file: close the file using the close() method
example code
def read_file(file_path):
try:
with open(file_path, 'r') as file:
content = file.read()
print("Content of the file:")
print(content)
except FileNotFoundError:
print(f"Error: The file '{file_path}' was not found.")

read_file('sample.txt')
To write into a file
Open the file: Use the open() function with the file path and mode 'w' for writing
Write to the file: Use methods like write() to write data to the file.
Close the file: close the file using the close() method to save changes
example code
def write_to_file(file_path, lines):
try:
with open(file_path, 'w') as file:
for line in lines:
file.write(line + "\n")
print(f"Successfully wrote {len(lines)} lines to '{file_path}'.")
except IOError:
print(f"Error writing to file '{file_path}'.")

lines_to_write = ["First line", "Second line", "Third line"]
write_to_file('output.txt', lines_to_write)

# references

https://docs.python.org/
https://www.w3schools.com/python/
https://www.geeksforgeeks.org/python-exception-handling/

# Submission Guidelines:

- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].
