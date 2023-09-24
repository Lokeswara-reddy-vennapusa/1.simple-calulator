# 1.simple-calulator

Display Menu:

You print the menu of available operations directly to the console using print statements:

print("1 Addition")
print("2 Subtraction")
print("3 Multiplication")
print("4 Division")

User Input:

The program takes user input for their choice of operation (choice) and the two numbers to perform the operation on (num1 and num2).


choice = input("Enter your choice: ")
num1 = float(input("Enter Number 1: "))
num2 = float(input("Enter Number 2: "))

Like before, it converts the input numbers to floating-point values.


Operation Execution:

The program uses conditional statements (if, elif, and else) to determine which operation the user selected and then performs the operation directly within the print statement.


if choice == "1":
    print(num1, "+", num2, "=", (num1 + num2))
elif choice == "2":
    print(num1, "-", num2, "=", (num1 - num2))
elif choice == "3":
    print(num1, "*", num2, "=", (num1 * num2))
elif choice == "4":
    if num2 == 0.0:
        print("Divide by 0 Error")
    else:
        print(num1, "/", num2, "=", (num1 / num2))
else:
    print("Invalid choice")
    
If the user attempts to divide by zero, it prints "Divide by 0 Error."

If the user chooses an invalid operation (other than 1, 2, 3, or 4), it prints "Invalid choice."

Your code effectively implements a simple calculator program and handles basic error cases such as division by zero and invalid input choices.
