[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15340817&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   Python is a powerful yet beginner-friendly high-level, general-purpose programming language.
Examples;
   Web Development: Frameworks like Django and Flask make Python a powerful tool for building dynamic websites and web applications.

   Data Science and Machine Learning: Python's libraries like NumPy, Pandas, and Scikit-learn are instrumental in data analysis, manipulation, and machine learning tasks.

   Scripting and Automation: Python is excellent for automating repetitive tasks, saving developers and system administrators significant time.

   Scientific Computing: Python's ease of use and powerful libraries make it popular for scientific research and computations.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

Installing Python on Windows:

Download the installer:

Head to the official Python download page (https://www.python.org/downloads/).
Download the latest stable version of Python 3. 

Run the installer:

Double-click the downloaded installer file .
In the installation wizard, it's recommended to check the box "Add Python 3.x to PATH." This allows you to run Python commands from anywhere in your command prompt.

Verifying Installation:
Open Command Prompt:

Search for "Command Prompt" in the Start menu and launch it.
Check Python version:

Type python --version and press Enter. If Python is installed correctly, it should display the installed version number (e.g., Python 3.10.x).
Setting Up a Virtual Environment 

Install venv module (if not already installed):

Open a command prompt and type python -m pip install venv. This installs the venv module, which is used to create virtual environments.

Create a virtual environment:

Navigate to your desired project directory in the command prompt.
Type python -m venv my_venv (replace my_venv with your preferred virtual environment name). This creates a directory named my_venv containing all the necessary files for your isolated Python environment.
Activate the virtual environment:

Windows: my_venv\Scripts\activate.bat
This activates the virtual environment, and your command prompt will typically show the name of the active environment in parentheses before the prompt (e.g., (my_venv) >).
Verify activation:

To confirm activation, try running python --version again. It should show the Python version installed within the virtual environment.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   print("Hello, World!")
   print function: This built-in function displays the message passed within the parentheses on the console.
   "" (Double quotes): These enclose the text "Hello, World!" which is a string in Python. Strings represent textual data.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   Integers (int): Represent whole numbers, positive, negative, or zero (e.g., 10, -5, 0).
   Floats (float): Represent decimal numbers (e.g., 3.14, -10.25).
   Complex Numbers (complex): Represent numbers with a real and imaginary part (e.g., 3+5j, where j represents the imaginary unit).
   Strings (str): Represent sequences of characters (text) enclosed in quotes (single '' or double "" are common).
   Booleans (bool): Represent logical values, True or False.
   # Integer
age = 25

# Float
pi = 3.14159

# String
name = "Alice"
# Boolean
is_raining = True

print("Age:", age)
print("Pi:", pi)
print("Name:", name)
print("Fruits:", fruits)
print("Is raining:", is_raining)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
if-else statement: This is the basic structure for conditional statements.
The if clause checks a condition.
If the condition is true, the indented code block following if executes.
An optional else clause provides an alternative code block if the condition is false.

or loop: This iterates over a sequence of elements (like a list or string).
The for clause defines a loop variable that takes on each value in the sequence one by one.

   def is_even(number):
  if number % 2 == 0:
    return True
  else:
    return False

# Use a for loop to iterate through a list
numbers = [1, 2, 3, 4, 5]
for num in numbers:
  if is_even(num):
    print(num, "is even")
  else:
    print(num, "is odd")

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions in Python are reusable blocks of code that perform specific tasks. They offer several advantages:

Reusability: You can define a function once and call it multiple times throughout your program, reducing code duplication and making your code more concise.
Modularity: Functions break down complex programs into smaller, manageable parts, improving readability and maintainability.
Encapsulation: Functions can group related code and data together, hiding internal implementation details and promoting better organization.
   # Example usage
result = sum_numbers(5, 3)
print("The sum is:", result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   Lists: Ordered, mutable collections of elements enclosed in square brackets []. Elements can be of various data types, and you can access them by their index (position) in the list. 

   Dictionaries: Unordered, mutable collections of key-value pairs enclosed in curly braces {}. Keys must be unique and immutable (like strings or numbers), while values can be of any data type. Dictionaries are efficient for storing data associated with names or labels, allowing you to retrieve values by their corresponding keys.

# Create a list of numbers
numbers = [1, 5, 3, 2, 4]

# Access elements by index
first_number = numbers[0]  # Accesses the first element (index 0)
print("First number:", first_number)

# Modify elements in the list
numbers[2] = 10  # Changes the value at index 2
print("Modified list:", numbers)

# Create a dictionary with key-value pairs
person = {
  "name": "Alice",
  "age": 30,
  "city": "New York"
}

# Access elements by key
name = person["name"]  # Access the value associated with the key "name"
print("Name:", name)

# Add new key-value pairs
person["occupation"] = "Software Engineer"
print("Updated dictionary:", person)

# Loop through a dictionary (iterates over keys)
for key in person:
  print(key, ":", person[key])

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

Exception handling in Python is a mechanism to manage errors (exceptions) that may occur during program execution. It allows you to write robust code that anticipates potential issues and gracefully recovers from them. Here's how it works:

try block: This block contains the code that might raise an exception.
except block: This block handles specific exceptions that occur within the try block. You can have multiple except blocks to handle different types of exceptions.
finally block (optional): This block executes regardless of whether an exception occurs or not. It's commonly used to release resources or perform cleanup tasks.

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

Modules:

Single Python files (.py) containing functions, variables, and classes.
Promote code reuse by letting you import functionalities from other files.
Packages:

Collections of related modules organized in directories.
Provide a hierarchical structure to avoid naming conflicts and improve maintainability.
Importing Modules:

Entire Module:

Python
import module_name
Use code with caution.
content_copy
Use module_name.identifier to access elements (e.g., math.sqrt(16)).

Specific Elements:

Python
from module_name import function_name, variable_name
Use code with caution.
content_copy
Use elements directly (e.g., sqrt(16) if sqrt is imported from math).

Example Using math Module:

Python
import math

result = math.sqrt(16)
print("Square root of 16:", result)

pi = math.pi
print("Value of pi:", pi)
Use code with caution.
content_copy
Packages:

Use dot notation to import from packages (e.g., package_name.sub_package.module_name).
   

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Reading:

Open the file in read mode ('r') using open(filename, 'r').
Read the content:
Use read() to get the entire file as a string.
Use readline() to read each line individually.
Use readlines() to get all lines as a list.
Close the file with close() to release resources.

Writing:

Open the file in write mode ('w') or append mode ('a') using open(filename, mode).
Write mode creates a new file or overwrites existing content.
Append mode adds content to the end of an existing file.
Write the data using write(data).
Close the file with close() to ensure data is saved.
Example (Reading):

Python
def read_file(filename):
  try:
    with open(filename, 'r') as file:
      contents = file.read()
      print(contents)
  except FileNotFoundError:
    print("Error: File not found.")
Use code with caution.
content_copy
Example (Writing):

Python
def write_list_to_file(filename, data):
  try:
    with open(filename, 'w') as file:
      for item in data:
        file.write(item + "\n")
  except FileNotFoundError:
    print("Error: Could not create file.")


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


