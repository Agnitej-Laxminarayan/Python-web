Regular Expressions in Python
=============================

Regular expressions (regex) are sequences of characters that define a search pattern. They are commonly used for string matching and manipulation. In Python, the ``re`` module is used to work with regular expressions.

Basic Syntax for Regular Expressions
------------------------------------

.. code-block:: python

    import re

    pattern = r'your_regex_pattern'
    string = "your target string"

    # To find all matches
    matches = re.findall(pattern, string)

    # To search for a match
    match = re.search(pattern, string)

    # To replace matches with a replacement string
    replaced_string = re.sub(pattern, replacement, string)

    # To split a string by a regex pattern
    split_list = re.split(pattern, string)

Examples
--------

Program 1
~~~~~~~~~~~~

This example demonstrates how to find all email addresses in a given string.

.. code-block:: python

    import re

    pattern = r'[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+'
    string = "Contact us at support@example.com or sales@example.co.uk."

    matches = re.findall(pattern, string)

    print("Found email addresses:", matches)

Program 2
~~~~~~~~~~~~~~~~~

This example demonstrates how to validate a complex password. The password must be at least 8 characters long, include at least one uppercase letter, one lowercase letter, one digit, and one special character.

.. code-block:: python

    import re

    def validate_password(password):
        # Regex pattern for a valid password
        pattern = r'^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,}$'

        match = re.match(pattern, password)
        if match:
            return "Password is valid."
        else:
            return "Password is invalid."

    # Test the function
    passwords = ["Password123!", "invalidPass", "Pass!2", "Valid$Pass123"]
    results = [validate_password(pw) for pw in passwords]

    for pw, result in zip(passwords, results):
        print(str(pw) + str(result))

.. note::

    Regular expressions can be very powerful, but they can also be very complex and difficult to understand. It's often a good idea to use tools like regex testers to build and test your regular expressions before using them in your code.