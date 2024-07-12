.. _looping:

Looping in Python
=================

Introduction to Looping
-----------------------

Looping is a fundamental concept in programming that allows you to execute a block of code repeatedly. Python supports two types of loops: ``for`` loops and ``while`` loops.

**`for` Loop**

The ``for`` loop iterates over a sequence (such as a list, tuple, dictionary, set, or string) and executes the block of code for each item in the sequence.

**Syntax:**

.. code-block:: python

    for item in sequence:
        # Code to execute

**Example:**

.. code-block:: python

    # Iterating over a list
    fruits = ["apple", "banana", "cherry"]
    for fruit in fruits:
        print(fruit)  # Output: apple banana cherry

    # Iterating over a range of numbers
    for i in range(5):
        print(i)  # Output: 0 1 2 3 4

**Explanation:**

In the first example, the ``for`` loop iterates over the list ``fruits`` and prints each fruit. In the second example, the ``for`` loop iterates over a range of numbers from 0 to 4 and prints each number.

**`while` Loop**

The ``while`` loop executes a block of code as long as a specified condition is ``True``.

**Syntax:**

.. code-block:: python

    while condition:
        # Code to execute

**Example:**

.. code-block:: python

    # Printing numbers from 0 to 4
    i = 0
    while i < 5:
        print(i)  # Output: 0 1 2 3 4
        i += 1

**Explanation:**

In this example, the ``while`` loop executes the block of code as long as ``i`` is less than 5. The value of ``i`` is incremented by 1 in each iteration.

.. note::
   - The ``for`` loop is more suitable for iterating over a sequence.
   - The ``while`` loop is more suitable for repeating a block of code while a condition is ``True``.

.. warning::
   - Be careful with ``while`` loops; if the condition never becomes ``False``, it will result in an infinite loop.

.. _range:


Introduction to `range`
-----------------------

The `range` function in Python is used to generate a sequence of numbers. It is commonly used in loops to iterate over a sequence of numbers. The `range` function can take one, two, or three arguments:

1. ``range(stop)``: Generates numbers from 0 up to, but not including, ``stop``.
2. ``range(start, stop)``: Generates numbers from ``start`` up to, but not including, ``stop``.
3. ``range(start, stop, step)``: Generates numbers from ``start`` up to, but not including, ``stop``, with a step value of ``step``.

**Syntax:**

.. code-block:: python

    range(stop)
    range(start, stop)
    range(start, stop, step)

**Example:**

.. code-block:: python

    # Using range with one argument
    for i in range(5):
        print(i, end=" ")  # Output: 0 1 2 3 4

    print()  # New line

    # Using range with two arguments
    for i in range(1, 6):
        print(i, end=" ")  # Output: 1 2 3 4 5

    print()  # New line

    # Using range with three arguments
    for i in range(1, 10, 2):
        print(i, end=" ")  # Output: 1 3 5 7 9

**Explanation:**

In the example above, we use the `range` function in three different ways:
- ``range(5)`` generates numbers from 0 to 4.
- ``range(1, 6)`` generates numbers from 1 to 5.
- ``range(1, 11, 2)`` generates numbers from 1 to 9 with a step of 2.

.. note::
   - The `range` function is often used in ``for`` loops to iterate over a sequence of numbers.

.. warning::
   - The `stop` value is not included in the generated sequence. That is 5,6,11 not included in the generated sequence.