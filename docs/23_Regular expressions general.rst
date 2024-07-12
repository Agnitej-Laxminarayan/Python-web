Regular Expressions
===================

Regular expressions, often abbreviated as regex or regexp, are sequences of characters that form a search pattern. They are used for pattern matching within strings and are commonly used in tasks such as search, replace, and validation.

Basic Syntax
------------

- **Literal Characters:** Match themselves exactly and do not have a special meaning in the regex syntax. For example, ``abc`` matches the string "abc".
- **Metacharacters:** Characters with special meanings, such as ``.``, ``^``, ``$``, ``*``, ``+``, ``?``, ``{}``, ``[]``, ``()``, ``|``, ``\``.

Common Metacharacters and Their Meanings
----------------------------------------

- ``.`` : Matches any single character except a newline.
- ``^`` : Matches the start of a string.
- ``$`` : Matches the end of a string.
- ``*`` : Matches 0 or more repetitions of the preceding element.
- ``+`` : Matches 1 or more repetitions of the preceding element.
- ``?`` : Matches 0 or 1 repetition of the preceding element.
- ``{n}`` : Matches exactly n repetitions of the preceding element.
- ``{n,}`` : Matches n or more repetitions of the preceding element.
- ``{n,m}`` : Matches between n and m repetitions of the preceding element.
- ``[]`` : Matches any one of the characters inside the brackets.
- ``|`` : Matches either the expression before or the expression after the ``|``.
- ``()`` : Groups multiple tokens together and creates a capture group.
- ``\`` : Escapes a metacharacter.

Special Sequences
-----------------

- ``\d`` : Matches any digit