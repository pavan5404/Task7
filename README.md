
# Task 7: Basic Sales Summary using Python and SQLite

# Objective

This project demonstrates how to:

* Connect Python to a SQLite database
* Run SQL queries from Python
* Load data into a pandas DataFrame
* Print basic sales summaries
* Visualize revenue data with a bar chart using matplotlib

# Tools Used

* Python
* SQLite3 (built-in)
* pandas
* matplotlib
* Jupyter Notebook / Python script

# Dataset

A small SQLite database `sales_data.db` was used, containing one table named `sales` with columns such as:

* `product`
* `quantity`
* `price`

# What the Script Does

* Connects to the SQLite database using `sqlite3`
* Executes an SQL query to summarize sales:

  ```sql
  SELECT product, SUM(quantity) AS total_qty, SUM(quantity * price) AS revenue FROM sales GROUP BY product
  ```
* Loads the results into a pandas DataFrame
* Prints the summarized data
* Plots a bar chart of revenue by product using matplotlib
* Saves the chart as `sales_chart.png`

# Output

* Printed summary table in the terminal
* Bar chart showing revenue per product

