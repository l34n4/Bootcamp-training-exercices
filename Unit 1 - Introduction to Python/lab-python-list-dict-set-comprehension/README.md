# Lab: List, Dict, and Set Comprehension

This lab builds on the previous inventory and order management exercise by incorporating Python comprehension techniques to simplify and optimize the code. It covers initializing inventory, gathering customer orders, calculating total price, and updating inventory dynamically.

The lab includes:
- **Inventory Initialization**: Use dictionary comprehension to set product quantities.
- **Customer Orders**: Use set comprehension to gather orders dynamically.
- **Total Price Calculation**: Use list comprehension to prompt for product prices and calculate the total.
- **Inventory Updates**: Automatically remove products with zero quantities using dictionary comprehension.
- **Order Statistics**: Display the total products ordered and percentage of products ordered.

## Example Workflow
1. The user inputs quantities for products in inventory.
2. The user specifies the number of orders and products they want to add.
3. For each product, the user provides the price, and the program calculates the total price.
4. The inventory updates dynamically, and order statistics are displayed.

### Example Output
```plaintext
Enter the quantity of t-shirts available: 5
Enter the quantity of mugs available: 4
Enter the name of a product: hat
Do you want to add another product? no

Order Statistics:
Total Products Ordered: 2
Percentage of Products Ordered: 40.0%

Updated Inventory:
t-shirt: 5
mug: 4
hat: 2

Total Price: $15.0
