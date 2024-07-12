.. _dsa_strings:

Data Structures and Algorithms: Strings
=======================================

Data structure 
Definition - A data structure is a particular way of organizing, managing, and storing data in a computer so that it can be accessed and modified efficiently. Data structures define the relationship between data, the operations that can be performed on the data, and the ways in which the data can be manipulated.

Introduction to Strings
-----------------------

Strings are a fundamental data type in Python and many other programming languages. They represent sequences of characters and are used to store and manipulate text. In Python, strings are immutable, meaning that once created, they cannot be changed.

Strings as Data Structures
--------------------------

Strings are also considered data structures because they store and manage collections of characters. As a data structure, a string provides various operations to access, manipulate, and process the characters it contains. This dual nature of strings as both a data type and a data structure makes them versatile and powerful tools in programming.

Basic String Operations
-----------------------

**Creating Strings:**

.. code-block:: python

    # Single quotes
    str1 = 'Hello, World!'

    # Double quotes
    str2 = "Hello, World!"

    # Triple quotes for multi-line strings
    str3 = """This is a
    multi-line string."""

**Accessing Characters in a String:**

.. code-block:: python

    text = "Python"
    first_char = text[0]  # 'P'
    last_char = text[-1]  # 'n'

**String Concatenation:**

.. code-block:: python

    # Using the + operator
    greeting = "Hello, " + "World!"

**String Repetition:**

.. code-block:: python

    # Using the * operator
    repeat = "Python! " * 3  # 'Python! Python! Python! '

String Methods
--------------

Strings come with a variety of built-in methods for common operations.

**Common String Methods:**

.. code-block:: python

    text = "Hello, World!"

    # Convert to uppercase
    upper_text = text.upper()  # 'HELLO, WORLD!'

    # Convert to lowercase
    lower_text = text.lower()  # 'hello, world!'

    # Find a substring
    position = text.find("World")  # 7

    # Replace a substring
    replaced_text = text.replace("World", "Python")  # 'Hello, Python!'

    # Check if a string starts with a substring
    is_start = text.startswith("Hello")  # True

    # Check if a string ends with a substring
    is_end = text.endswith("!")  # True

Advanced String Operations
--------------------------

**String Slicing:**

String slicing allows you to extract a substring from a string.

.. code-block:: python

    text = "Data Structures and Algorithms"
    substring = text[5:16]  # 'Structures'

**String Splitting and Joining:**

.. code-block:: python

    # Splitting a string into a list of words
    text = "Python is awesome"
    words = text.split()  # ['Python', 'is', 'awesome']

    # Joining a list of words into a single string
    sentence = " ".join(words)  # 'Python is awesome'

**String Formatting:**

String formatting allows you to create strings with dynamic content.

.. code-block:: python

    name = "Alice"
    age = 30
    intro = "My name is " + name + " and I am " + str(age) + " years old."  # 'My name is Alice and I am 30 years old.'

Important Notes and Warnings
----------------------------

.. note::
   - Strings in Python are immutable. Once created, you cannot change the content of a string.
   - String methods often return a new string instead of modifying the original string.

.. warning::
   - Be careful when accessing string indices. An ``IndexError`` will be raised if you try to access an index that is out of range.
   - Using string concatenation (``+``) in loops can lead to performance issues. Consider using ``str.join()`` for better performance.