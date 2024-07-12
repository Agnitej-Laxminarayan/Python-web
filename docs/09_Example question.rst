Example question
=================

Question
--------

Write a Python program that takes three inputs from the user: two integers and an operator (+, -, *, /). 
The program should evaluate the expression and print the result along with a detailed explanation of the operation performed. 
Use try and except blocks to handle invalid inputs and possible errors, such as division by zero or invalid operator. 
If the user enters an invalid operator, the program should print an error message.

Solution
--------

.. _solution-python-code:

.. code-block:: python
   :linenos:

   try:
       # Take the first integer input from the user
       num1 = int(input("Enter the first integer: "))

       # Take the operator input from the user
       operator = input("Enter an operator (+, -, *, /): ")

       # Take the second integer input from the user
       num2 = int(input("Enter the second integer: "))

       # Evaluate the expression based on the operator
       if operator == '+':
           result = num1 + num2
           operation = "Addition"
       elif operator == '-':
           result = num1 - num2
           operation = "Subtraction"
       elif operator == '*':
           result = num1 * num2
           operation = "Multiplication"
       elif operator == '/':
           if num2 == 0:
               print("Error: Division by zero.")
           else:
               result = num1 / num2
               operation = "Division"
       else:
           print("Error: Invalid operator. Please use one of the following operators: +, -, *, /")
           exit()

       # Print the result with a detailed explanation
       print(str(num1) + " " + operator + " " + str(num2) + " = " + str(result) + ". " + operation + " was performed.")

   except:
       print("Error: Invalid input or an unexpected error occurred. Please enter valid numerical values and a valid operator.")
