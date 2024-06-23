[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15315945&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   Python is a versatile, high-level programming language known for its simplicity, readability, and extensive libraries, making it popular for web development (Django, Flask), data analysis (Pandas, NumPy), artificial intelligence (TensorFlow, PyTorch), and scripting tasks.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

     -To install Python on your operating system, begin by visiting the official Python website (python.org) and downloading the latest version suitable for your OS (Windows, macOS, Linux). Run the installer, ensuring to check the box that adds Python to PATH during installation on Windows. For macOS and Linux, Python is typically pre-installed; however, using the installer ensures the latest version. After installation, open a terminal (or command prompt on Windows) and type python --version to verify installation. To set up a virtual environment, use python -m venv <path_to_virtual_environment> to create a new environment. Activate it with source <path_to_virtual_environment>/bin/activate on macOS/Linux or <path_to_virtual_environment>\Scripts\activate on Windows.
3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
            # Simple Python program to print "Hello, World!" to the console
print("Hello, World!")
    print: Python built-in function used to output text or variables to the console.
"Hello, World!": String literal enclosed in double quotes, representing the text to be printed.
#: Denotes a comment in Python, ignored by the interpreter, used for adding notes or explanations to the code.
4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
     -Basic data types in Python:

   Integer (int): Represents whole numbers without decimal points, e.g., 5, -10.
   Float (float): Represents numbers with decimal points, e.g., 3.14, -0.001.
   String (str): Represents sequences of characters enclosed in single ' or double " quotes, e.g., 'hello', "Python".
   Boolean (bool): Represents truth values True or False.
   List: Represents an ordered collection of items, mutable, and can contain elements of different data types, e.g., [1, 2, 'apple'].
   Tuple: Represents an ordered collection of items, immutable, e.g., (1, 2, 'banana').
    (dict): Represents a collection of key-value pairs, e.g., {'name': 'Alice', 'age': 30}.
              #Example script demonstrating different data types:
              # Define variables of different data types
integer_var = 42
float_var = 3.14
string_var = 'Hello, Python!'
boolean_var = True
list_var = [1, 2, 3, 'apple']
tuple_var = (4, 5, 'banana')
dictionary_var = {'name': 'Alice', 'age': 30}

# Print out each variable
print("Integer variable:", integer_var)
print("Float variable:", float_var)
print("String variable:", string_var)
print("Boolean variable:", boolean_var)
print("List variable:", list_var)
print("Tuple variable:", tuple_var)
print("Dictionary variable:", dictionary_var)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
    Conditional statements (if-else):

Used to make decisions based on conditions.
Syntax: `if condition:
Code to execute if condition is true
else:
# Code to execute if condition is false`
# Example of an if-else statement
age = 20
if age >= 18:
    print("You are an adult.")
else:
    print("You are not yet an adult.")
Loops (for loop):

Used to iterate over a sequence (like lists, tuples, strings, etc.).
Syntax: `for element in sequence:
Code to execute for each element
# Example of a for loop
fruits = ['apple', 'banana', 'cherry']
for fruit in fruits:
    print(fruit)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
Functions in Python:Functions are blocks of reusable code that perform a specific task.
                    They help in organizing code into manageable parts and promote code reuse.
                    Functions are defined using the def keyword followed by a function name and parameters.
                    They can optionally return a value using the return statement.
         Example of a function that returns the sum of two arguments:
# Define a function that takes two arguments and returns their sum
def sum_two_numbers(a, b):
    return a + b

# Example of calling the function
result = sum_two_numbers(3, 5)
print("The sum is:", result)


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
          Lists in Python:
Ordered collection of items.
Accessed by index.
Mutable (can be changed).
Example: numbers = [1, 2, 3, 4, 5]
Dictionaries in Python:

Unordered collection of key-value pairs.
Accessed by keys.
Mutable (values can be changed, keys are immutable).
Example: person = {'name': 'Alice', 'age': 30}

# Create a list of numbers
numbers = [1, 2, 3, 4, 5]

# Create a dictionary of person's information
person = {'name': 'Alice', 'age': 30, 'city': 'New York'}

# Print the list and dictionary
print("List of numbers:", numbers)
print("Dictionary of person:", person)

# Accessing elements in list
print("First number in the list:", numbers[0])

# Accessing elements in dictionary
print("Name of the person:", person['name'])

# Modifying elements in list
numbers[0] = 10
print("Updated list of numbers:", numbers)

# Modifying elements in dictionary
person['age'] = 31
print("Updated dictionary of person:", person)

# Adding elements to list
numbers.append(6)
print("List after adding a number:", numbers)

# Adding elements to dictionary
person['gender'] = 'female'
print("Dictionary after adding a key-value pair:", person)

# Removing elements from list
numbers.remove(3)
print("List after removing a number:", numbers)

# Removing elements from dictionary
del person['city']
print("Dictionary after removing a key:", person)






8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   Exception handling in Python:
Exception handling is a mechanism to handle runtime errors gracefully.
It prevents the program from crashing when an error occurs.
Errors are caught using try, except blocks.

# Example of exception handling
try:
    num1 = int(input("Enter a number: "))
    num2 = int(input("Enter another number: "))
    result = num1 / num2
    print("Result:", result)
except ValueError:
    print("Error: Please enter a valid integer.")
except ZeroDivisionError:
    print("Error: Division by zero is not allowed.")
finally:
    print("Execution completed.")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   Modules in Python:
Modules are files containing Python code that define functions, classes, and variables.
They allow for better organization and reuse of code.
You can create your own modules or use built-in modules

Packages in Python:
Packages are directories containing multiple modules.
They have a special file named __init__.py which indicates it's a package.
They help in structuring large Python projects.

Importing and using a module in Python:
Use import module_name to import a module.
Access functions and variables using module_name.function() or module_name.variable.

# Example of importing and using the math module
import math

# Calculate the square root of a number
num = 25
sqrt_value = math.sqrt(num)
print("Square root of", num, "is:", sqrt_value)

# Calculate the factorial of a number
factorial_value = math.factorial(5)
print("Factorial of 5 is:", factorial_value)


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Reading from a file:
Use open() function with mode 'r' to open a file for reading.
Use methods like read(), readline(), or readlines() to read content.
Always close the file with close() or use it within a with statement.

# Example of reading from a file and printing its content
filename = 'sample.txt'

with open(filename, 'r') as file:
    content = file.read()

print("Content of", filename, ":")
print(content)


# Example of writing a list of strings to a file
filename = 'output.txt'
lines = ['Line 1\n', 'Line 2\n', 'Line 3\n']

with open(filename, 'w') as file:
    for line in lines:
        file.write(line)

print("Data written to", filename)





