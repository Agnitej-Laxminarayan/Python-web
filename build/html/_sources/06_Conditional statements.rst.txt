Conditional Statements
================================

Conditional statements are used to perform different actions based on different conditions. Python supports the usual logical conditions from mathematics:

- Equals: `a == b`
- Not Equals: `a != b`
- Less than: `a < b`
- Less than or equal to: `a <= b`
- Greater than: `a > b`
- Greater than or equal to: `a >= b`

Types of Conditional Statements:
---------------------------------
1. **if Statement**
2. **elif Statement**
3. **else Statement**

Syntax:
-------
- **if Statement:**

  .. code-block:: python

     if condition:
         statement

- **elif Statement:**

  .. code-block:: python

     if condition:
         statement
     elif another_condition:
         another_statement

- **else Statement:**

  .. code-block:: python

     if condition:
         statement
     else:
         statement

Example:
--------

.. code-block:: python

   x = 10

   if x > 0:
       print("x is a positive number")
   elif x == 0:
       print("x is zero")
   else:
       print("x is a negative number")

.. note::
   Indentation is crucial in Python. All statements within the same block of code must have the same indentation level.