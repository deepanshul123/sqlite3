SQLite3 Project Summary
Objective:
Use Python with SQLite3 to:
•	Create a sales database (sales_data.db)
•	Insert and retrieve data using SQL
•	Display the results using print()
________________________________________
Steps Performed:
1. Imported Required Library:
import sqlite3
•	Utilized Python’s built-in library to interact with SQLite.
2. Connected to Database:
conn = sqlite3.connect('sales_data.db')
cursor = conn.cursor()
•	Connected to or created a SQLite database named sales_data.db.
3. Created Sales Table (if not exists):
CREATE TABLE IF NOT EXISTS sales (
    product TEXT,
    quantity INTEGER,
    price REAL
)
•	Defined a table named sales with fields:
o	product: name of the product (text)
o	quantity: number of units sold (integer)
o	price: price per unit (real number)
4. Verified Table Creation:
•	Successful execution returned a cursor object like <sqlite3.Cursor at 0x...>, confirming the command ran without errors.
________________________________________
Next Recommended Steps:
If not already completed:
•	Insert sample data using executemany()
•	Retrieve and display data using SELECT * FROM sales
•	Optionally, visualize results using pandas or matplotlib
