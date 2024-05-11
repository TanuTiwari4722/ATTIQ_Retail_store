# ATTIQ Retails Case Study 
Tables used :
* Customers
* Products
* Stores
* Regions
* Calendar
* Returns
* Transactions including a folder combination of two tables for 1997 and 1998.

# Data Cleaning Process 
1. Customers Table : Checked data types of columns. Merged The first name and last name columns to get full name.Extracted Year to get the Year from birthdate. Added a conditional column to get if a person has children or not.

2. Products Table : Checked data types of columns. Applied statistic(distinct) function to get distinct product brands. Added a calculated column for discounted price as : 
discounted_price = Products[product_retail_price] * 0.9. Replaced "null" values with zeros in both the "recyclable" and "low-fat" columns.

3. Stores Table : Checked data type of columns, Add a calculated column named "full_address", by merging "store_city", "store_state", and "store_country", separated by a comma and space.Add a calculated column named "area_code", by extracting the characters before the dash ("-") in the "store_phone" field.

4. Regions Table : Headers promoted. Checked Data Types.
5. Calendars : Headers promoted. Added custom columns, Start of week, name of day, name of month, start of month, Quarter of year, year columns.
6. Returns Table : Headers promoted. Checked Data Types.
7. Transactions : Added two tables via a folder value, Connect to the folder path, and choose "Edit" vs. Combine and Edit.

