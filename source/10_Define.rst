.. _functions:

Functions
=========

Defining Functions
------------------

Functions are reusable blocks of code that perform a specific task. In Python, you define a function using the ``def`` keyword followed by the function name and parentheses ``()``. The function body is indented.

**Syntax:**

.. code-block:: python

    def function_name(parameters):
        # function body
        statement(s)

**Example:**

.. code-block:: python

    def greet(name):
        print(f"Hello, {name}!")

**Explanation:**

In the example above, we define a function named ``greet`` that takes one parameter ``name`` and prints a greeting message.

.. _simple_calculator:

Example: Simple Calculator
---------------------------

Let's create a simple calculator that can perform addition, subtraction, multiplication, and division using functions.

**Syntax and Example Usage:**

.. code-block:: python

    # Function definitions
    def add(a, b):
        return a + b

    def subtract(a, b):
        return a - b

    def multiply(a, b):
        return a * b

    def divide(a, b):
        if b == 0:
            return "Error: Division by zero!"
        return a / b

    # Example usage of the calculator functions
    num1 = 10
    num2 = 5

    print(str(num1) + " + " + str(num2) + " = " + str(add(num1, num2)))
    print(str(num1) + " - " + str(num2) + " = " + str(subtract(num1, num2)))
    print(str(num1) + " * " + str(num2) + " = " + str(multiply(num1, num2)))
    print(str(num1) + " / " + str(num2) + " = " + str(divide(num1, num2)))

**Explanation:**

In this example, we define four functions: ``add``, ``subtract``, ``multiply``, and ``divide``. Each function takes two parameters and performs the corresponding arithmetic operation. The ``divide`` function includes error handling for division by zero. The example usage demonstrates how to call these functions and print the results using string concatenation with the ``+`` operator.

.. note::
   - Each function returns the result of the operation.
   - The ``divide`` function checks if the divisor is zero to avoid a runtime error.

.. warning::
   - Make sure to handle edge cases, such as division by zero, to prevent unexpected errors.

.. note::
   - Functions help in modularizing code and improving readability.
   - Indentation is important in Python; it defines the scope of the function.

.. warning::
   - Make sure to use the correct indentation; otherwise, you will get an ``IndentationError``.