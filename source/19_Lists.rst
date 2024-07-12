Lists
=====

A list is a collection which is ordered and changeable. In Python, lists are written with square brackets.

Creating a List
---------------

.. code-block:: python
   :linenos:

   # Creating a simple list
   my_list = [1, 2, 3, 4, 5]

   # Creating a list with mixed data types
   mixed_list = [1, "Hello", 3.14, True]

Accessing List Items
---------------------

List items are indexed, the first item has index [0], the second item has index [1], etc.

.. code-block:: python
   :linenos:

   # Accessing items in a list
   print(my_list[0])  # Output: 1
   print(mixed_list[1])  # Output: Hello

.. note::
   List indices start at 0. Attempting to access an index that doesn't exist will raise an IndexError.

Modifying List Items
--------------------

.. code-block:: python
   :linenos:

   # Modifying items in a list
   my_list[1] = 20
   print(my_list)  # Output: [1, 20, 3, 4, 5]

Adding Items to a List
----------------------

.. code-block:: python
   :linenos:

   # Using append() to add an item
   my_list.append(6)
   print(my_list)  # Output: [1, 20, 3, 4, 5, 6]

   # Using insert() to add an item at a specified index
   my_list.insert(2, "new")
   print(my_list)  # Output: [1, 20, 'new', 3, 4, 5, 6]

Removing Items from a List
--------------------------

.. code-block:: python
   :linenos:

   # Using remove() to remove a specific item
   my_list.remove(20)
   print(my_list)  # Output: [1, 'new', 3, 4, 5, 6]

   # Using pop() to remove an item at a specified index
   my_list.pop(2)
   print(my_list)  # Output: [1, 'new', 4, 5, 6]

   # Using del to delete an item at a specified index
   del my_list[0]
   print(my_list)  # Output: ['new', 4, 5, 6]

.. warning::
   The del statement can delete entire lists as well. Use with caution.

List Comprehension
------------------

List comprehensions provide a concise way to create lists.

.. code-block:: python
   :linenos:

   # List comprehension example
   squares = [x**2 for x in range(10)]
   print(squares)  # Output: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

List Methods
------------

Here are some common methods you can use with lists:

- ``append()``: Adds an element at the end of the list
- ``extend()``: Adds the elements of a list (or any iterable), to the end of the current list
- ``insert()``: Adds an element at the specified position
- ``remove()``: Removes the first item with the specified value
- ``pop()``: Removes the element at the specified position
- ``clear()``: Removes all the elements from the list
- ``index()``: Returns the index of the first element with the specified value
- ``count()``: Returns the number of elements with the specified value
- ``sort()``: Sorts the list
- ``reverse()``: Reverses the order of the list
- ``copy()``: Returns a copy of the list

Example Usage of List Methods
-----------------------------

.. code-block:: python
   :linenos:

   my_list = [3, 1, 4, 1, 5, 9, 2]

   # Append
   my_list.append(6)
   print(my_list)  # Output: [3, 1, 4, 1, 5, 9, 2, 6]

   # Extend
   my_list.extend([7, 8])
   print(my_list)  # Output: [3, 1, 4, 1, 5, 9, 2, 6, 7, 8]

   # Insert
   my_list.insert(2, 10)
   print(my_list)  # Output: [3, 1, 10, 4, 1, 5, 9, 2, 6, 7, 8]

   # Remove
   my_list.remove(1)
   print(my_list)  # Output: [3, 10, 4, 1, 5, 9, 2, 6, 7, 8]

   # Pop
   my_list.pop(3)
   print(my_list)  # Output: [3, 10, 4, 5, 9, 2, 6, 7, 8]

   # Clear
   my_list.clear()
   print(my_list)  # Output: []

   # Re-initializing for further examples
   my_list = [3, 1, 4, 1, 5, 9, 2]

   # Index
   print(my_list.index(9))  # Output: 5

   # Count
   print(my_list.count(1))  # Output: 2

   # Sort
   my_list.sort()
   print(my_list)  # Output: [1, 1, 2, 3, 4, 5, 9]

   # Reverse
   my_list.reverse()
   print(my_list)  # Output: [9, 5, 4, 3, 2, 1, 1]

   # Copy
   copied_list = my_list.copy()
   print(copied_list)  # Output: [9, 5, 4, 3, 2, 1, 1]