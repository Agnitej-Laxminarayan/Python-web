Dictionaries
============

A dictionary is a collection which is unordered, changeable, and indexed. In Python, dictionaries are written with curly brackets, and they have keys and values.

Syntax
------

.. code-block:: python
   :linenos:

   # Creating an empty dictionary
   my_dict = {}

   # Creating a dictionary with initial values
   my_dict = {"key1": "value1", "key2": "value2"}

Creating a Dictionary
---------------------

.. code-block:: python
   :linenos:

   # Creating a simple dictionary
   my_dict = {"name": "John", "age": 30, "city": "New York"}

   # Creating a dictionary with mixed data types
   mixed_dict = {"key1": 123, "key2": [1, 2, 3], "key3": (4, 5, 6)}

Accessing Dictionary Items
--------------------------

You can access the items of a dictionary by referring to its key name, inside square brackets.

.. code-block:: python
   :linenos:

   # Accessing items in a dictionary
   print(my_dict["name"])  # Output: John
   print(mixed_dict["key2"])  # Output: [1, 2, 3]

.. note::
   If the key does not exist, attempting to access it will raise a KeyError.

Modifying Dictionary Items
--------------------------

.. code-block:: python
   :linenos:

   # Modifying items in a dictionary
   my_dict["age"] = 31
   print(my_dict)  # Output: {"name": "John", "age": 31, "city": "New York"}

Adding Items to a Dictionary
----------------------------

.. code-block:: python
   :linenos:

   # Adding items to a dictionary
   my_dict["email"] = "john@example.com"
   print(my_dict)  # Output: {"name": "John", "age": 31, "city": "New York", "email": "john@example.com"}

Removing Items from a Dictionary
--------------------------------

.. code-block:: python
   :linenos:

   # Using pop() to remove a specific item
   my_dict.pop("age")
   print(my_dict)  # Output: {"name": "John", "city": "New York", "email": "john@example.com"}

   # Using del to remove a specific item
   del my_dict["city"]
   print(my_dict)  # Output: {"name": "John", "email": "john@example.com"}

   # Using clear() to empty the dictionary
   my_dict.clear()
   print(my_dict)  # Output: {}

.. warning::
   The ``clear()`` method will remove all elements from the dictionary. Use it with caution.

Dictionary Methods
------------------

Here are some common methods you can use with dictionaries:

- ``clear()``: Removes all elements from the dictionary
- ``copy()``: Returns a copy of the dictionary
- ``fromkeys()``: Returns a dictionary with the specified keys and value
- ``get()``: Returns the value of the specified key
- ``items()``: Returns a list containing a tuple for each key-value pair
- ``keys()``: Returns a list containing the dictionary's keys
- ``pop()``: Removes the element with the specified key
- ``popitem()``: Removes the last inserted key-value pair
- ``setdefault()``: Returns the value of the specified key. If the key does not exist, insert the key, with the specified value
- ``update()``: Updates the dictionary with the specified key-value pairs
- ``values()``: Returns a list of all the values in the dictionary

Example Usage of Dictionary Methods
-----------------------------------

.. code-block:: python
   :linenos:

   my_dict = {"name": "John", "age": 30, "city": "New York"}

   # Clear
   my_dict.clear()
   print(my_dict)  # Output: {}

   # Re-initializing for further examples
   my_dict = {"name": "John", "age": 30, "city": "New York"}

   # Copy
   copied_dict = my_dict.copy()
   print(copied_dict)  # Output: {'name': 'John', 'age': 30, 'city': 'New York'}

   # Fromkeys
   keys = ('key1', 'key2', 'key3')
   value = 0
   new_dict = dict.fromkeys(keys, value)
   print(new_dict)  # Output: {'key1': 0, 'key2': 0, 'key3': 0}

   # Get
   print(my_dict.get("name"))  # Output: John

   # Items
   print(my_dict.items())  # Output: dict_items([('name', 'John'), ('age', 30), ('city', 'New York')])

   # Keys
   print(my_dict.keys())  # Output: dict_keys(['name', 'age', 'city'])

   # Pop
   my_dict.pop("age")
   print(my_dict)  # Output: {'name': 'John', 'city': 'New York'}

   # Popitem
   my_dict.popitem()
   print(my_dict)  # Output: {'name': 'John'}

   # Setdefault
   my_dict.setdefault("age", 31)
   print(my_dict)  # Output: {'name': 'John', 'age': 31}

   # Update
   my_dict.update({"city": "New York", "email": "john@example.com"})
   print(my_dict)  # Output: {'name': 'John', 'age': 31, 'city': 'New York', 'email': 'john@example.com'}

   # Values
   print(my_dict.values())  # Output: dict_values(['John', 31, 'New York', 'john@example.com'])

Difference between Lists and Dictionaries
------------------------------------------

Lists
-----

- A list is a collection which is ordered and changeable.
- Lists are written with square brackets ``[]``.
- List items are indexed, with the first item having index ``[0]``.
- Lists allow duplicate members.
- Elements are accessed using their index positions.

Dictionaries
------------

- A dictionary is a collection which is unordered, changeable, and indexed.
- Dictionaries are written with curly brackets ``{}``.
- Dictionary items are accessed by their key, not by index.
- Dictionaries do not allow duplicate keys.
- Keys must be unique and immutable (e.g., strings, numbers, tuples), but values can be of any type.

Key Differences
---------------

1. **Order:**
   - Lists maintain the order of items.
   - Dictionaries do not maintain the order of items (prior to Python 3.7). From Python 3.7 onwards, dictionaries maintain the order of insertion.

2. **Accessing Elements:**
   - List elements are accessed by their index.
   - Dictionary elements are accessed by their key.

3. **Syntax:**
   - Lists use square brackets ``[]``.
   - Dictionaries use curly brackets ``{}`` with key-value pairs separated by colons ``:``.

4. **Duplication:**
   - Lists allow duplicate values.
   - Dictionaries do not allow duplicate keys.

Example
-------

.. code-block:: python
   :linenos:

   # List example
   my_list = [1, 2, 3, 4, 5]

   # Accessing list items
   print(my_list[0])  # Output: 1

   # Dictionary example
   my_dict = {"name": "John", "age": 30, "city": "New York"}

   # Accessing dictionary items
   print(my_dict["name"])  # Output: John

