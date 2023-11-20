# Data Cleaning and Merging using VLOOKUP, INDEX_MATCH, XLOOKUP:

Dataset : The 'product_sales_db.xlsx' file contains 3 tables:
	- orders
	- products
	- customer

1. "orders": This table contains information about the orders placed by customers, including the order ID, date of the order, 

	        customer ID, product ID, and quantity of the product ordered.

2. "products": This table contains information about the products offered by the company, including the product ID,

	          product name, nutritional information (calories, protein, carbs, and fat), and price in Indian Rupees.

3. "customer": This table contains information about the customers who have placed orders, including their customer ID and name.

# Objectives by the Stakeholders

## Objective 1:

For orders table:

	- Eliminate duplicate 'order_id' to prevent double-counting in data analysis.

	- Convert the data type of 'product_id' from number to Text.

	- To address data entry issues, replace the incorrect entries in the 'qty' field that end with "Q" and append the corrected values as necessary.

	- Substitute any empty values in the 'qty' column with the text 'Not Available'.

For the products table:

	- Remove all the extra leading and trailing spaces in product_name. (Hint: use TRIM() function)

	- split the 'price (in Rs)' column at the '₹' symbol and extract the numerical values. 

	  Rename the columns appropriately after completing this task.

For the customer table:

	- Convert all customer names to lowercase.

	- Copy all customer name values, then paste them permanently using 'Paste Special' -> 'Values'.

## Objective 2:

1. Retrieve all the customer names that correspond to their respective 'customer_id' listed in the orders table.

2. Retrieve all the product names that correspond to their respective 'product_id' listed in the orders table.

3. Obtain the corresponding 'price (in Rs)' of the products listed in the orders table.

4. Calculate the product of 'qty' and 'price (in INR)'# Excel-Analytics
