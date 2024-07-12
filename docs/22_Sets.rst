Sets
====

A set is a collection which is unordered, unchangeable (but you can add or remove items), and unindexed. Sets are written with curly brackets.

Creating a Set
--------------

.. code-block:: python
   :linenos:

   # Creating a simple set
   my_set = {1, 2, 3, 4, 5}

   # Creating a set with mixed data types
   mixed_set = {1, "Hello", 3.14, True}

   # Creating an empty set
   empty_set = set()

Accessing Set Items
-------------------

You cannot access items in a set by referring to an index, since sets are unordered. But you can loop through the set items using a ``for`` loop, or ask if a specified value is present in a set by using the ``in`` keyword.

.. code-block:: python
   :linenos:

   # Looping through a set
   for item in my_set:
       print(item)

   # Checking if an item exists in a set
   print(1 in my_set)  # Output: True

Adding Items to a Set
---------------------

.. code-block:: python
   :linenos:

   # Using add() to add an item
   my_set.add(6)
   print(my_set)  # Output: {1, 2, 3, 4, 5, 6}

   # Using update() to add multiple items
   my_set.update([7, 8])
   print(my_set)  # Output: {1, 2, 3, 4, 5, 6, 7, 8}

Removing Items from a Set
-------------------------

.. code-block:: python
   :linenos:

   # Using remove() to remove a specific item
   my_set.remove(2)
   print(my_set)  # Output: {1, 3, 4, 5, 6, 7, 8}

   # Using discard() to remove a specific item
   my_set.discard(3)
   print(my_set)  # Output: {1, 4, 5, 6, 7, 8}

   # Using pop() to remove an arbitrary item
   my_set.pop()
   print(my_set)  # Output: {4, 5, 6, 7, 8}

   # Using clear() to empty the set
   my_set.clear()
   print(my_set)  # Output: set()

Set Methods
-----------

Here are some common methods you can use with sets:

- ``add()``: Adds an element to the set
- ``clear()``: Removes all elements from the set
- ``copy()``: Returns a copy of the set
- ``difference()``: Returns a set containing the difference between two or more sets
- ``difference_update()``: Removes the items in this set that are also included in another specified set
- ``discard()``: Removes the specified item
- ``intersection()``: Returns a set, that is the intersection of two other sets
- ``intersection_update()``: Removes the items in this set that are not present in other specified sets
- ``isdisjoint()``: Returns whether two sets have a intersection or not
- ``issubset()``: Returns whether another set contains this set or not
- ``issuperset()``: Returns whether this set contains another set or not
- ``pop()``: Removes an element from the set
- ``remove()``: Removes the specified element
- ``symmetric_difference()``: Returns a set with the symmetric differences of two sets
- ``symmetric_difference_update()``: Inserts the symmetric differences from this set and another
- ``union()``: Returns a set containing the union of sets
- ``update()``: Update the set with the union of this set and others

Example Usage of Set Methods
----------------------------

.. code-block:: python
   :linenos:

   set1 = {1, 2, 3, 4}
   set2 = {3, 4, 5, 6}

   # Add
   set1.add(5)
   print(set1)  # Output: {1, 2, 3, 4, 5}

   # Clear
   set1.clear()
   print(set1)  # Output: set()

   # Copy
   set3 = set2.copy()
   print(set3)  # Output: {3, 4, 5, 6}

   # Difference
   print(set1.difference(set2))  # Output: set()

   # Difference Update
   set1.difference_update(set2)
   print(set1)  # Output: set()

   # Discard
   set2.discard(3)
   print(set2)  # Output: {4, 5, 6}

   # Intersection
   print(set1.intersection(set2))  # Output: set()

   # Intersection Update
   set1.intersection_update(set2)
   print(set1)  # Output: set()

   # Is Disjoint
   print(set1.isdisjoint(set2))  # Output: True

   # Is Subset
   print(set1.issubset(set2))  # Output: True

   # Is Superset
   print(set2.issuperset(set1))  # Output: True

   # Pop
   print(set2.pop())  # Output: 4 (or any other random element)

   # Remove
   set2.remove(5)
   print(set2)  # Output: {6}

   # Symmetric Difference
   print(set1.symmetric_difference(set2))  # Output: {1, 2, 3, 4}

   # Symmetric Difference Update
   set1.symmetric_difference_update(set2)
   print(set1)  # Output: {1, 2, 3, 4}

   # Union
   print(set1.union(set2))  # Output: {1, 2, 3, 4, 5, 6}

   # Update
   set1.update(set2)
   print(set1)  # Output: {1, 2, 3, 4, 5, 6}