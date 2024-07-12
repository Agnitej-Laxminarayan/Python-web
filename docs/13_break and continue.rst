.. _break_and_continue:

break and continue
==================

Introduction to `break` and `continue`
--------------------------------------

The `break` and `continue` statements in Python are used to control the flow of loops. They provide a way to modify the behavior of loops based on specific conditions.

**break Statement**

The `break` statement is used to exit a loop prematurely when a certain condition is met. It terminates the loop and transfers control to the next statement after the loop.

**Syntax:**

.. code-block:: python

    for item in sequence:
        if condition:
            break
        # Code to execute

    while condition:
        if condition:
            break
        # Code to execute

**Example 1:**

.. code-block:: python

    # Using break in a for loop
    for i in range(10):
        if i == 5:
            break
        print(i)  # Output: 0 1 2 3 4

    # Using break in a while loop
    i = 0
    while i < 10:
        if i == 5:
            break
        print(i)  # Output: 0 1 2 3 4
        i += 1

**Example 2:**

.. code-block:: python

    # Finding the first number in a list that is divisible by both 3 and 5
    numbers = [1, 2, 7, 10, 15, 20, 30]
    for num in numbers:
        if num % 3 == 0 and num % 5 == 0:
            print("First number divisible by both 3 and 5 is:", num)  # Output: First number divisible by both 3 and 5 is: 15
            break

**`continue` Statement**

The `continue` statement is used to skip the current iteration of a loop and move to the next iteration. It causes the loop to jump to the next iteration immediately.

**Syntax:**

.. code-block:: python

    for item in sequence:
        if condition:
            continue
        # Code to execute

    while condition:
        if condition:
            continue
        # Code to execute

**Example 1:**

.. code-block:: python

    # Using continue in a for loop
    for i in range(10):
        if i % 2 == 0:
            continue
        print(i)  # Output: 1 3 5 7 9

    # Using continue in a while loop
    i = 0
    while i < 10:
        i += 1
        if i % 2 == 0:
            continue
        print(i)  # Output: 1 3 5 7 9

**Example 2:**

.. code-block:: python

    # Printing non-prime numbers from 2 to 20
    for num in range(2, 21):
        is_prime = True
        for i in range(2, num):
            if num % i == 0:
                is_prime = False
                break
        if is_prime:
            continue
        print(num, "is not a prime number")  # Output: 4 is not a prime number, 6 is not a prime number, ...

**Explanation:**

In the examples provided:
- The `break` statement is used to exit the loop when a specific condition is met.
- The `continue` statement is used to skip the current iteration of the loop when a specific condition is met.

.. note::
   - The `break` statement is used to exit a loop prematurely.
   - The `continue` statement is used to skip the current iteration and proceed to the next iteration.

.. warning::
   - Use `break` and `continue` statements cautiously to avoid unexpected behavior in loops.