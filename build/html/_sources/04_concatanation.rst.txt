Concatenation
=======================

Concatenation in Python refers to the operation of joining two or more sequences end-to-end. This operation is most commonly used with strings but can also be applied to lists, tuples, and other sequence types.

String Concatenation
--------------------

### Using the `+` Operator

The simplest way to concatenate strings in Python is by using the `+` operator.

#### Example

.. code-block:: python

    str1 = "Hello"
    str2 = "World"
    result = str1 + " " + str2
    print(result)

Output:

::

    Hello World

.. note::

    When concatenating strings using the `+` operator, ensure that all operands are strings. Otherwise, you may encounter a TypeError.

#### Example of TypeError

.. code-block:: python

    # This will raise a TypeError
    num = 42
    result = "The answer is " + num
    print(result)

Error:

::

    TypeError: can only concatenate str (not "int") to str

#### Corrected Example

.. code-block:: python

    # Convert the number to a string
    num = 42
    result = "The answer is " + str(num)
    print(result)

Output:

::

    The answer is 42

List Concatenation
------------------

Lists can be concatenated using the `+` operator.

### Using the `+` Operator

#### Example

.. code-block:: python

    list1 = [1, 2, 3]
    list2 = [4, 5, 6]
    result = list1 + list2
    print(result)

Output:

::

    [1, 2, 3, 4, 5, 6]

.. warning::

    Be cautious when concatenating lists using the `+` operator, as it creates a new list. This can be inefficient for large lists.

#### Inefficient Example

.. code-block:: python

    # Concatenating large lists
    large_list1 = [i for i in range(100000)]
    large_list2 = [i for i in range(100000, 200000)]
    result = large_list1 + large_list2
    print(len(result))  # Output: 200000

Tuple Concatenation
-------------------

Tuples can be concatenated using the `+` operator.

### Using the `+` Operator

#### Example

.. code-block:: python

    tuple1 = (1, 2, 3)
    tuple2 = (4, 5, 6)
    result = tuple1 + tuple2
    print(result)

Output:

::

    (1, 2, 3, 4, 5, 6)

.. note::

    Since tuples are immutable, concatenating tuples using the `+` operator creates a new tuple.

Program Example
---------------

Here's a complete program that demonstrates concatenation with strings, lists, and tuples:

.. code-block:: python

    # String concatenation
    str1 = "Hello"
    str2 = "World"
    str_result = str1 + " " + str2
    print("String Concatenation:", str_result)

    # List concatenation
    list1 = [1, 2, 3]
    list2 = [4, 5, 6]
    list_result = list1 + list2
    print("List Concatenation:", list_result)

    # Tuple concatenation
    tuple1 = (1, 2, 3)
    tuple2 = (4, 5, 6)
    tuple_result = tuple1 + tuple2
    print("Tuple Concatenation:", tuple_result)

Output
------

.. code-block:: text

    String Concatenation: Hello World
    List Concatenation: [1, 2, 3, 4, 5, 6]
    Tuple Concatenation: (1, 2, 3, 4, 5, 6)

Summary
-------

Concatenation is a fundamental operation in Python that allows you to join sequences such as strings, lists, and tuples. By using the `+` operator, you can efficiently combine multiple sequences into one. Be mindful of data types and performance considerations when performing concatenation.