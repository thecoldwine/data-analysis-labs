# Lab 1

For this lab you will need:

1) SQLite
2) git
3) For later steps you can use any IDE for SQL (Dbeaver, SQLiteStudio, etc.)

Note: you will need to use CLI (command line interface) for this lab, so you are encouraged to use WSL (Windows Subsystem for Linux) with Ubuntu.
It will help you to understand actual tools better rather than just clicking on buttons in IDE / web browser. I know, it is taxing, you'll thank me later.

https://learn.microsoft.com/en-us/windows/wsl/install

## Task 1

Download the dataset from here:

https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales

The dataset is in CSV format and has following columns:
- Invoice id
- Branch: Branch of supercenter (3 branches are available identified by A, B and C).
- City: Location of supercenters
- Customer type
- Gender of customer
- Product line: General item categorization groups - Electronic accessories, Fashion accessories, Food and beverages, Health and beauty, Home and lifestyle, Sports and travel

Create a new database and import the dataset into a table.

1) Run sqlite3 in CLI - `sqlite3`
2) Create a new database - `.open supermarket.db`
3) Import the dataset - `.mode csv` and `.import supermarket_sales.csv supermarket_sales`
4) Test if your import was successful - `SELECT * FROM supermarket_sales LIMIT 10;`

## Task 2

Write a query that will return the total number of sales for each product line. Export this list to a CSV file.

1) Turn headers on `.headers on`
2) Set output mode to CSV `.mode csv`
3) Export the result of the query to CSV file `.output sales_by_product_line.csv`
4) Write the query (the output will be saved to the file).
5) Turn off output to CSV file `.output`

## Task 3

Write a query which will return best selling product line for each branch. Export this list to a CSV file.

1) Turn headers on `.headers on`
2) Set output mode to CSV `.mode csv`
3) Export the result of the query to CSV file `.output best_selling_product_line_by_branch.csv`
4) Write the query (the output will be saved to the file).
5) Turn off output to CSV file `.output`

## Task 4

Every product has a price. Write a query which will return the total revenue for each product line. Export this list to a CSV file.

Write a query which will return best selling product line for each branch. Export this list to a CSV file.

1) Turn headers on `.headers on`
2) Set output mode to CSV `.mode csv`
3) Export the result of the query to CSV file `.output best_selling_product_line_by_branch.csv`
4) Write the query (the output will be saved to the file).
5) Turn off output to CSV file `.output`