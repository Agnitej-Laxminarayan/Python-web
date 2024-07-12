Example code
=================================

**Question: 1**

Write a Python code to open the file in read format and count how many lines start with `example.l@gmail.com`.

**Answer:**

To accomplish this task, we can use the following Python code. The code will open the file in read mode and count the number of lines that start with `example.l@gmail.com`.

**Python Code:**

.. code-block:: python

   # Define the file path
   file_path = r"C:/Users/YourUsername/Downloads/mails.txt"

   # Initialize the count
   count = 0

   # Open the file in read mode
   with open(file_path, "r") as file:
       lines = file.readlines()
       for line in lines:
           if line.startswith("example.l@gmail.com"):
               count += 1

   print("Number of lines starting with 'example.l@gmail.com':" + str(count));


.. note::
   Make sure to replace `YourUsername` with your actual Windows username in the file path.When you use a backslash in a file path, 
   such as "C:\Users\NLC3KOR\Downloads\mails.txt", 
   Python tries to interpret \U as the start of a Unicode escape sequence, which it cannot recognize or decode properly in this context,
   leading to the unicodeescape error.To fix this,
   Use a Raw String: By prefixing the string with r, you tell Python to treat the backslashes as literal characters and not as escape 
   characters.

.. warning::
   Ensure that the file `mails.txt` is downloaded and placed in the specified directory before running the script.


**Question: 2**

2. Write a Program to insert a mail-id example.l@gmail.com at 19th line.

.. code-block:: python

    # Define the file path
    file_path = r"C:\Users\Username\Downloads\mails.txt"

    # The email to be added
    email = "example.l@gmail.com"

    # Read the existing lines from the file
    with open(file_path, "r") as file:
        lines = file.readlines()

    # Ensure there are at least 18 lines in the file
    while len(lines) < 18:
        lines.append("\n")

    # Insert the email at the 19th line (index 18)
    if len(lines) >= 18:
        lines.insert(18, email + "\n")

    # Write the modified lines back to the file
    with open(file_path, "w") as file:
        file.writelines(lines)

    print("Email added to the 19th line.")

.. warning::
    Opening a file in write mode (`"w"`) will erase its previous contents. Make sure to read and manipulate the file content in memory before writing it back to avoid data loss.