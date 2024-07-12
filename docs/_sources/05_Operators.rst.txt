Operators
====================

Operators are special symbols in Python that perform operations on variables and values. Python supports a variety of operators that can be categorized into several types:

1. Arithmetic Operators
2. Comparison Operators
3. Logical Operators
4. Bitwise Operators
5. Assignment Operators
6. Identity Operators
7. Membership Operators

Arithmetic Operators
---------------------

Arithmetic operators are used to perform mathematical operations like addition, subtraction, multiplication, etc.

.. list-table::
   :header-rows: 1

   * - **Operator**
     - **Description**
     - **Example**
   * - ``+``
     - Addition
     - ``x + y`` (Adds ``x`` and ``y``)
   * - ``-``
     - Subtraction
     - ``x - y`` (Subtracts ``y`` from ``x``)
   * - ``*``
     - Multiplication
     - ``x * y`` (Multiplies ``x`` and ``y``)
   * - ``/``
     - Division
     - ``x / y`` (Divides ``x`` by ``y``)
   * - ``%``
     - Modulus
     - ``x % y`` (Returns the remainder when ``x`` is divided by ``y``)
   * - ``**``
     - Exponentiation
     - ``x ** y`` (Returns ``x`` raised to the power of ``y``)
   * - ``//``
     - Floor Division
     - ``x // y`` (Returns the floor of the division of ``x`` by ``y``)

.. warning::
   Division by zero will raise a ``ZeroDivisionError``.

.. code-block:: python

    x = 10
    y = 0
    # This will raise ZeroDivisionError
    result = x / y

Comparison Operators
---------------------

Comparison operators are used to compare two values.

.. list-table::
   :header-rows: 1

   * - **Operator**
     - **Description**
     - **Example**
   * - ``==``
     - Equal to
     - ``x == y`` (True if ``x`` is equal to ``y``)
   * - ``!=``
     - Not equal to
     - ``x != y`` (True if ``x`` is not equal to ``y``)
   * - ``>``
     - Greater than
     - ``x > y`` (True if ``x`` is greater than ``y``)
   * - ``<``
     - Less than
     - ``x < y`` (True if ``x`` is less than ``y``)
   * - ``>=``
     - Greater than or equal to
     - ``x >= y`` (True if ``x`` is greater than or equal to ``y``)
   * - ``<=``
     - Less than or equal to
     - ``x <= y`` (True if ``x`` is less than or equal to ``y``)

.. note::
   Comparison operators return Boolean values (``True`` or ``False``).

.. code-block:: python

    x = 10
    y = 5
    print(x > y)  # Output: True
    print(x == y) # Output: False

Logical Operators
------------------

Logical operators are used to combine conditional statements.

.. list-table::
   :header-rows: 1

   * - **Operator**
     - **Description**
     - **Example**
   * - ``and``
     - Logical AND
     - ``x and y`` (True if both ``x`` and ``y`` are true)
   * - ``or``
     - Logical OR
     - ``x or y`` (True if either ``x`` or ``y`` is true)
   * - ``not``
     - Logical NOT
     - ``not x`` (True if ``x`` is false)

.. code-block:: python

    x = True
    y = False
    print(x and y) # Output: False
    print(x or y)  # Output: True
    print(not y)   # Output: True

Bitwise Operators
------------------

Bitwise operators are used to perform bit-level operations.

.. list-table::
   :header-rows: 1

   * - **Operator**
     - **Description**
     - **Example**
   * - ``&``
     - Bitwise AND
     - ``x & y`` (Performs bitwise AND on ``x`` and ``y``)
   * - ``|``
     - Bitwise OR
     - ``x | y`` (Performs bitwise OR on ``x`` and ``y``)
   * - ``^``
     - Bitwise XOR
     - ``x ^ y`` (Performs bitwise XOR on ``x`` and ``y``)
   * - ``~``
     - Bitwise NOT
     - ``~x`` (Performs bitwise NOT on ``x``)
   * - ``<<``
     - Bitwise left shift
     - ``x << y`` (Shifts ``x`` left by ``y`` bits)
   * - ``>>``
     - Bitwise right shift
     - ``x >> y`` (Shifts ``x`` right by ``y`` bits)

.. code-block:: python

    x = 10  # 1010 in binary
    y = 4   # 0100 in binary
    print(x & y)  # Output: 0 (0000 in binary)
    print(x | y)  # Output: 14 (1110 in binary)

Assignment Operators
---------------------

Assignment operators are used to assign values to variables.

.. list-table::
   :header-rows: 1

   * - **Operator**
     - **Description**
     - **Example**
   * - ``=``
     - Assign
     - ``x = y`` (Assigns value of ``y`` to ``x``)
   * - ``+=``
     - Add and assign
     - ``x += y`` (Adds ``y`` to ``x`` and assigns the result to ``x``)
   * - ``-=``
     - Subtract and assign
     - ``x -= y`` (Subtracts ``y`` from ``x`` and assigns the result to ``x``)
   * - ``*=``
     - Multiply and assign
     - ``x *= y`` (Multiplies ``x`` by ``y`` and assigns the result to ``x``)
   * - ``/=``
     - Divide and assign
     - ``x /= y`` (Divides ``x`` by ``y`` and assigns the result to ``x``)
   * - ``%=``
     - Modulus and assign
     - ``x %= y`` (Calculates the modulus of ``x`` and ``y`` and assigns the result to ``x``)
   * - ``**=``
     - Exponentiation and assign
     - ``x **= y`` (Calculates the exponentiation of ``x`` and ``y`` and assigns the result to ``x``)
   * - ``//=``
     - Floor division and assign
     - ``x //= y`` (Performs floor division on ``x`` and ``y`` and assigns the result to ``x``)

.. code-block:: python

    x = 10
    x += 5  # Equivalent to x = x + 5
    print(x)  # Output: 15

Identity Operators
-------------------

Identity operators are used to compare the memory locations of two objects.

.. list-table::
   :header-rows: 1

   * - **Operator**
     - **Description**
     - **Example**
   * - ``is``
     - Is
     - ``x is y`` (True if ``x`` and ``y`` are the same object)
   * - ``is not``
     - Is not
     - ``x is not y`` (True if ``x`` and ``y`` are not the same object)

.. note::
   Identity operators are often used to compare objects, not just their values.

.. code-block:: python

    x = [1, 2, 3]
    y = x
    z = [1, 2, 3]
    print(x is y)    # Output: True
    print(x is z)    # Output: False

Membership Operators
---------------------

Membership operators are used to test if a sequence contains a certain value.

.. list-table::
   :header-rows: 1

   * - **Operator**
     - **Description**
     - **Example**
   * - ``in``
     - In
     - ``x in y`` (True if ``x`` is in ``y``)
   * - ``not in``
     - Not in
     - ``x not in y`` (True if ``x`` is not in ``y``)

.. code-block:: python

    x = [1, 2, 3]
    print(2 in x)     # Output: True
    print(5 not in x) # Output: True

Summary
-------

Understanding and effectively using operators in Python is crucial for performing various computations and making decisions in your code. Each type of operator serves a specific purpose and offers different functionalities. By mastering operators, you can write more efficient and readable Python code.