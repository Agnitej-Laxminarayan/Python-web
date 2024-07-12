.. _find_largest_and_smallest:

Example code
=================================

This program allows the user to input a series of numbers. When the user types "done!", the program will print the largest and smallest numbers from the input.

**Python Code:**

.. code-block:: python

    # Function to get user input and find the largest and smallest numbers
    def find_largest_and_smallest():
        largest = None
        smallest = None

        while True:
            user_input = input("Enter a number (or type 'done!' to finish): ")

            if user_input.lower() == "done!":
                break

            try:
                number = float(user_input)

                if largest is None or number > largest:
                    largest = number

                if smallest is None or number < smallest:
                    smallest = number

            except ValueError:
                print("Invalid input. Please enter a valid number.")

        if largest is not None and smallest is not None:
            print("Largest number:", largest)
            print("Smallest number:", smallest)
        else:
            print("No numbers were entered.")

    # Call the function
    find_largest_and_smallest()

**Explanation:**

1. The function ``find_largest_and_smallest()`` initializes ``largest`` and ``smallest`` to ``None``.
2. The ``while`` loop runs indefinitely until the user types "done!".
3. The user is prompted to enter a number. If the input is "done!", the loop breaks.
4. The input is converted to a float. If it's a valid number, the code checks if ``largest`` or ``smallest`` is ``None`` or if the number is larger than ``largest`` or smaller than ``smallest``. If so, it updates ``largest`` and ``smallest`` accordingly.
5. If the input is not a valid number, an error message is displayed.
6. After exiting the loop, the program checks if ``largest`` and ``smallest`` are not ``None``. If they are not ``None``, it prints the largest and smallest numbers. If no numbers were entered, a message is displayed indicating that no numbers were entered.