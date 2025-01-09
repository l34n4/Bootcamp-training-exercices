# Lab: Python Error Handling

## Objective

This lab focuses on practicing error handling in Python programs using `try`, `except`, `else`, and `finally` blocks, as well as raising custom exceptions. The goal is to enhance the robustness and reliability of your code by managing runtime errors effectively.

## Learning Goals

By completing this lab, you will be able to:

- Implement error handling techniques to manage runtime errors.
- Use the `try-except-else-finally` structure to handle exceptions gracefully.
- Raise exceptions when necessary to indicate that an error has occurred.
- Catch and handle specific exceptions using the `except` clause.
- Use multiple `except` clauses to handle different types of exceptions.

## Prerequisites

Before starting this lab, you should be familiar with:

- Data types, operators, and structures.
- Flow control (`if-else` statements and loops).
- Functions.
- Error handling in Python: `try`, `except`, `raise`.

## Instructions

1. **Basic Error Handling**:
   - Write a function that prompts the user for a number and handles invalid input (e.g., non-numeric values) using `try` and `except`.

2. **File Handling with Errors**:
   - Write a function that opens a file and handles errors such as `FileNotFoundError`. Ensure the file is closed properly, even if an exception occurs, using `try`, `except`, and `finally`.

3. **Custom Exceptions**:
   - Define a custom exception for a specific use case (e.g., when a value exceeds a predefined limit) and raise it appropriately within a function.

4. **Advanced Scenarios**:
   - Write a function that handles multiple exceptions in a single `try` block and uses nested `try-except` blocks to manage complex workflows.

## Example Code Snippet

```python
def divide_numbers():
    try:
        numerator = float(input("Enter the numerator: "))
        denominator = float(input("Enter the denominator: "))
        result = numerator / denominator
    except ValueError:
        print("Invalid input! Please enter numeric values.")
    except ZeroDivisionError:
        print("Error! Division by zero is not allowed.")
    else:
        print(f"The result is {result}")
    finally:
        print("Execution completed.")

divide_numbers()
