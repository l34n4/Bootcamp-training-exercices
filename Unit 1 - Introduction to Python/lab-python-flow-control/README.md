# Lab: Flow Control

## Objective

This lab enhances the functionality of a previous program that manages customer orders and inventory by introducing flow control concepts. The goal is to create a more efficient and user-friendly experience while practicing Python loops and conditional statements.

## Features

1. Replace repeated code with loops to improve efficiency.
2. Allow users to add as many products as they want to their orders by:
   - Asking the user if they want to add another product.
   - Continuing until the user indicates they are done.
3. Update inventory quantities only for the products that were ordered.

## Instructions

1. **Review Previous Code**:
   - Look at your code from the **Lab: Data Structures** and identify repetitive patterns.
   - Refactor the code to replace redundancy with loops.

2. **Dynamic Customer Orders**:
   - Prompt the user to enter the name of a product they want to order.
   - Add the product to the `customer_orders` set.
   - Ask if they want to add another product (`yes/no`).
   - Continue this process until the user inputs `no`.

3. **Selective Inventory Update**:
   - Subtract 1 from the quantity in inventory **only** for the products that are in `customer_orders`.

## Example Code Snippet

```python
# Example: Adding products dynamically to orders
while True:
    order = input(f"Enter a product you want to order ({', '.join(products)}): ").lower()
    if order not in products:
        print("Product not found. Please choose from the available products.")
        continue
    customer_orders.add(order)
    add_more = input("Do you want to add another product? (yes/no): ").lower()
    if add_more == "no":
        break

