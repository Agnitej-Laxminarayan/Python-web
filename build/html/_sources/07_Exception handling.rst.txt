Exception handling
========================

In Python, the `try` and `except` blocks are used to handle exceptions, which are errors that occur during the execution of a program. By using `try` and `except`, you can write code that gracefully handles errors and continues executing without crashing the program.

Syntax:
-------
.. code-block:: python

   try:
       # Code that might raise an exception
       statement
   except ExceptionType:
       # Code to handle the exception
       statement

Example:
--------
.. code-block:: python

   try:
       # Attempt to divide by zero
       result = 10 / 0
       print("The result is:", result)
   except ZeroDivisionError:
       # Handle the division by zero error
       print("Error: Division by zero is not allowed.")

Notes:
------
- The `try` block contains code that might raise an exception.
- The `except` block contains code that handles the exception.
- You can specify multiple `except` blocks to handle different types of exceptions.
- The `ExceptionType` can be any built-in or user-defined exception.