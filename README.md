Create a simple Python program that asks the user to input two numbers and a mathematical operation (addition, subtraction, multiplication, or division).
Perform the operation based on the user's input and print the result.
Example: If a user inputs 10, 5, and +, your program should display 10 + 5 = 15.

ANSWER:

def calculate(operation, num1, num2):
    if operation == 'add':
        return num1 + num2
    elif operation == 'subtract':
        return num1 - num2
    elif operation == 'multiply':
        return num1 * num2
    elif operation == 'divide':
        if num2 != 0:
            return num1 / num2
        else:
            return "Error: Division by zero is undefined."
    else:
        return "Unknown operation."

# Taking inputs from the user
num1 = int(input("Enter the first number: "))
num2 = int(input("Enter the second number: "))
operation = input("Enter the operation ('add', 'subtract', 'multiply', 'divide'): ")

result = calculate(operation, num1, num2)
print("The result is:", result)


def perform_operation(operation, num1, num2):
    if operation == '+':
        result = num1 + num2
        return f"{num1} + {num2} = {result}"
    elif operation == '-':
        result = num1 - num2
        return f"{num1} - {num2} = {result}"
    elif operation == '*':
        result = num1 * num2
        return f"{num1} * {num2} = {result}"
    elif operation == '/':
        if num2 != 0:
            result = num1 / num2
            return f"{num1} / {num2} = {result}"
        else:
            return "Error: Division by zero is not allowed."
    else:
        return "Invalid operation. Please choose '+', '-', '*', or '/'."
        
ANSWER:

# Calculate the sum
result = 10 + 5

# Display the result
print(f"{10} + {5} = {result}")
