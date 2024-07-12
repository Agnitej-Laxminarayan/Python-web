Tuples
======

A tuple is a collection which is ordered and unchangeable. Tuples are written with round brackets.

Creating a Tuple
----------------

.. code-block:: python
   :linenos:

   # Creating a simple tuple
   my_tuple = (1, 2, 3, 4, 5)

   # Creating a tuple with mixed data types
   mixed_tuple = (1, "Hello", 3.14, True)

   # Creating a tuple with a single item (note the comma)
   single_item_tuple = (1,)

Accessing Tuple Items
----------------------

Tuple items are indexed, the first item has index ``[0]``, the second item has index ``[1]``, etc.

.. code-block:: python
   :linenos:

   # Accessing items in a tuple
   print(my_tuple[0])  # Output: 1
   print(mixed_tuple[1])  # Output: Hello

Tuples are Unchangeable
-----------------------

Once a tuple is created, you cannot change its values. Tuples are unchangeable, meaning that we cannot change, add, or remove items after the tuple has been created.

Tuple Methods
-------------

Here are some common methods you can use with tuples:

- ``count()``: Returns the number of times a specified value occurs in a tuple
- ``index()``: Searches the tuple for a specified value and returns the position of where it was found

Example Usage of Tuple Methods
------------------------------

.. code-block:: python
   :linenos:

   my_tuple = (1, 2, 3, 4, 5, 1, 1, 2)

   # Count
   print(my_tuple.count(1))  # Output: 3

   # Index
   print(my_tuple.index(3))  # Output: 2

Advantages of Using Tuples
--------------------------

- **Immutability:** Tuples are immutable, meaning they cannot be changed after creation. This makes them useful for fixed data collections.
- **Performance:** Tuples are generally faster than lists for indexing and iteration.
- **Hashable:** Tuples can be used as keys in dictionaries, whereas lists cannot be used as dictionary keys.