``Comments and Print`` 
==============================================

Comments in Python
##################

Comments are an essential part of writing readable code. They allow you to explain the purpose of code sections and make it easier for others to understand your thought process.

Types of Comments:
------------------
1. **Single-line Comment:** A comment that occupies a single line.
2. **Multi-line Comment:** A comment that spans multiple lines.

Syntax:
-------

- **Single-line Comment:** Use the `#` symbol to start a single-line comment.

  .. code-block:: python

     # This is a single-line comment
     print("Hello, World!")  # This is a comment after a statement

- **Multi-line Comment:** Use triple quotes (`'''` or `"""`) for multi-line comments.

  .. code-block:: python

     '''
     This is a multi-line comment.
     It spans multiple lines.
     '''
     print("Hello, World!")

     """
     This is another multi-line comment.
     It also spans multiple lines.
     """

.. note::
   Comments are ignored by the Python interpreter and do not affect the execution of the code.

Print function
###############

The ``print`` function is one of the most commonly used functions in Python. It is used to output data to the standard output device (usually the screen).

Syntax
------

.. code-block:: python

    print(*objects, sep=' ', end='\n', file=sys.stdout)

Parameters
----------

- **objects**: An arbitrary number of objects to be printed. These can be strings, numbers, or other data types. Multiple objects are separated by a comma.
- **sep** (optional): A string inserted between the objects. The default is a space (' ').
- **end** (optional): A string appended after the last object. The default is a newline ('\n').
- **file** (optional): An object with a `write` method. The default is `sys.stdout`. This part will be discussed later in the document.

.. note::
   The `*objects` parameter allows the `print` function to accept multiple arguments and print them all at once, separated by the `sep` parameter.

Examples
--------

Basic Usage
~~~~~~~~~~~

To print a simple message to the screen, you can use:

.. code-block:: python

    print("Hello, World!")

Output:

::

    Hello, World!

Printing Multiple Objects
~~~~~~~~~~~~~~~~~~~~~~~~~

You can print multiple objects by separating them with commas:

.. code-block:: python

    print("The answer is", 42)

Output:

::

    The answer is 42

.. note::
   The `print` function automatically converts non-string arguments to strings.

Using ``sep`` Parameter
~~~~~~~~~~~~~~~~~~~~~~~

The ``sep`` parameter allows you to change the separator between the objects:

.. code-block:: python

    print("apple", "banana", "cherry", sep=", ")

Output:

::

    apple, banana, cherry

.. warning::
   Setting `sep` to a value that is not a string will raise a `TypeError`.

Using ``end`` Parameter
~~~~~~~~~~~~~~~~~~~~~~~

The ``end`` parameter allows you to change what is printed at the end. The default is a newline character, but you can change it to something else:

.. code-block:: python

    print("Hello", end="")
    print("World")

Output:

::

    HelloWorld

If this `end` was not used, then the output would have been:

::

    Hello
    World

.. note::

   The `end` parameter is especially useful for creating progress bars or inline prints.