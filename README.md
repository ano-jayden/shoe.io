Shoe Inventory Management System

This project provides a Python-based Shoe Inventory Management System that reads, manages, and processes shoe inventory data. The program uses a structured class-based design with functionality to handle inventory operations efficiently.

Features

Read Shoes Data:

Reads inventory data from a text file (inventory.txt).

Populates a list of Shoe objects.

Capture Shoes:

Allows the user to manually input shoe details (country, code, product, cost, quantity) and adds them to the inventory.

View All Shoes:

Displays all the shoes in inventory in a tabulated format using the tabulate module.

Re-stock Shoes:

Identifies the shoe with the lowest quantity.

Allows the user to add to the stock of that shoe.

Search Shoe:

Searches for a shoe in the inventory by its code and displays its details.

Calculate Value per Item:

Computes the total value of each shoe type based on its cost and quantity.

Highest Quantity Shoe:

Identifies and displays the shoe with the highest quantity, marking it as "on sale."

Update Inventory File:

Updates the inventory.txt file to reflect the current state of the inventory.

File Structure

Python Script

The script (shoe_inventory.py) includes the following key components:

Shoe Class:

Represents a shoe with attributes: country, code, product, cost, and quantity.

Provides methods to get cost and quantity, and a string representation for display.

Functions:

read_shoes_data: Reads inventory from the inventory.txt file.

capture_shoes: Adds a new shoe to the inventory.

view_all: Displays inventory in a tabular format.

re_stock: Updates the stock of the shoe with the lowest quantity.

search_shoe: Finds and displays details of a specific shoe by its code.

value_per_item: Calculates and displays the total value of each shoe type.

highest_qty: Displays the shoe with the highest quantity.

update_inventory_file: Writes the updated inventory back to the file.

main_menu: Provides a user interface to access the program features.

Inventory File

The inventory.txt file contains the following columns:

Country: The country of origin of the shoe.

Code: The unique product code for the shoe.

Product: The name of the shoe.

Cost: The cost of the shoe.

Quantity: The number of units available.

Example:

Country,Code,Product,Cost,Quantity
South Africa,SKU44386,Air Max 90,2300,20
China,SKU90000,Jordan 1,3200,50
Vietnam,SKU63221,Blazer,1700,19
...

How to Use

Setup:

Install Python (if not already installed).

Install the tabulate module by running:

pip install tabulate

Prepare Data:

Ensure the inventory.txt file is in the same directory as the Python script.

Use the provided inventory format.

Run the Program:

Execute the Python script:

python shoe_inventory.py

Navigate the Menu:

Follow the on-screen prompts to choose from various options like viewing all shoes, restocking, searching, and more.

Dependencies

Python 3.6+

tabulate module (for table formatting)

Additional Notes

Ensure inventory.txt is always backed up before making major changes.

The program updates the file whenever restocking occurs to ensure data persistence.
