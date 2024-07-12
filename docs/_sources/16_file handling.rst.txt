File Handling
========================

File handling is an essential part of any programming language. Python provides various functions for creating, reading, updating, and deleting files.

Opening a File
--------------

The ``open()`` function is used to open a file. The syntax of the ``open()`` function is::

    file = open('filename', 'mode')

- ``filename``: The name of the file that you want to open.
- ``mode``: The mode in which you want to open the file. Some common modes include:
  - ``'r'``: Read mode (default)
  - ``'w'``: Write mode
  - ``'a'``: Append mode
  - ``'b'``: Binary mode

Example::

    file = open('example.txt', 'r')

.. note::

    If the file does not exist when opening in read mode, a FileNotFoundError is raised.

Closing a File
--------------

After performing operations on a file, it is important to close it using the ``close()`` method.

Example::

    file.close()

.. warning::

    Always close your files to free up system resources.

Writing to a File
-----------------

To write to a file, use the ``write()`` method.

Example::

    file = open('example.txt', 'w')
    file.write('Hello, World!')
    file.close()

.. note::

    If the file does not exist, it will be created.

Reading from a File
-------------------

To read the contents of a file, use the ``read()`` method.

Example::

    file = open('example.txt', 'r')
    content = file.read()
    print(content)
    file.close()

Using ``with`` Statement
------------------------

The ``with`` statement is used to wrap the file operations. It ensures that the file is properly closed after its suite finishes, even if an exception is raised.

Example::

    with open('example.txt', 'r') as file:
        content = file.read()
        print(content)

.. note::

    Using the ``with`` statement is considered a good practice as it handles file closing automatically.