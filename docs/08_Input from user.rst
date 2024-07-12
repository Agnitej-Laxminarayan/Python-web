Input from the User in Python
=============================

Taking input from the user is an essential part of many programs. In Python, you can use the `input()` function to read a string from standard input.

Syntax:
-------
.. code-block:: python

   variable = input("prompt")

Example:
--------
.. code-block:: python

   # Take a string input from the user
   name = input("Enter your name: ")
   print("Hello, " + name + "!")

Converting Input:
-----------------
By default, the `input()` function returns a string. If you need to convert the input to a different data type, you can use type conversion functions like `int()`, `float()`, etc.

Example:
--------
.. code-block:: python

   # Take an integer input from the user
   age = int(input("Enter your age: "))
   print("You are " + str(age) + " years old.")

Notes:
------
- Always validate and handle user input to prevent errors and unexpected behavior.
- Use `try` and `except` blocks to handle potential exceptions while converting input types.