.. _inbuilt_functions:

Inbuilt Functions
=================

Introduction to Inbuilt Functions
---------------------------------

Python provides numerous inbuilt functions that simplify tasks and enhance productivity. These functions are always available and do not require any import statements. Common inbuilt functions include ``len()``, ``type()``, ``print()``, ``input()``, ``str()``, ``int()``, ``float()``, ``list()``, ``dict()``, ``set()``, ``max()``, ``min()``, ``sum()``, ``sorted()``, ``range()``, and many more.

**Syntax and Examples:**

.. code-block:: python

    # Using inbuilt functions

    # Length of a string
    length = len("Hello, World!")
    print("Length of the string: " + str(length))  # Length of the string: 13

    # Type of a variable
    variable_type = type(123)
    print("Type of the variable: " + str(variable_type))  # Type of the variable: <class 'int'>

    # Convert a string to an integer
    number = int("10")
    print("Converted number: " + str(number))  # Converted number: 10

    # Convert an integer to a string
    string_number = str(123)
    print("String representation of the number: " + string_number)  # String representation of the number: 123

    # Create a list from a range
    numbers = list(range(1, 11))  # Range is explained in further topics
    print("List of numbers: " + str(numbers))  # List of numbers: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

    # Find the maximum and minimum values in a list
    max_value = max(numbers)
    min_value = min(numbers)
    print("Max value: " + str(max_value))  # Max value: 10
    print("Min value: " + str(min_value))  # Min value: 1

    # Calculate the sum of all elements in a list
    total_sum = sum(numbers)
    print("Sum of all numbers: " + str(total_sum))  # Sum of all numbers: 55

    # Sort a list
    sorted_numbers = sorted(numbers, reverse=True)
    print("Sorted numbers in descending order: " + str(sorted_numbers))  # Sorted numbers in descending order: [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]

**Explanation:**

In the example above, we use several inbuilt functions:
- ``len()`` to get the length of a string.
- ``type()`` to get the type of a variable.
- ``int()`` to convert a string to an integer.
- ``str()`` to convert an integer to a string.
- ``list()`` to create a list from a range.
- ``max()`` to find the maximum value in a list.
- ``min()`` to find the minimum value in a list.
- ``sum()`` to calculate the sum of all elements in a list.
- ``sorted()`` to sort a list.

.. note::
   - Inbuilt functions are very useful and can save time when writing code.

.. warning::
   - Make sure to use the correct data types when using these functions to avoid errors.