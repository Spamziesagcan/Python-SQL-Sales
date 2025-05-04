# 🛒 Python SQL Sales Summary Project

This project demonstrates how to create and analyze a simple sales database using **Python**, **SQLite**, **Pandas**, and **Matplotlib**. It is part of a data analyst internship task designed to help you practice database creation, SQL querying, and data visualization.

## 📂 Project Structure
├── create_sales_db.py # Script to create a superstore-style SQLite database with 20 rows
├── analyze_sales.py # Script to query and visualize revenue by product
├── sales_data.db # SQLite database file with sales data
├── product_vs_revenue.png # Bar chart of product vs revenue
└── README.md # Project documentation


## 🗃️ Database Schema

The `sales` table includes the following columns:

| Column    | Type    | Description                            |
|-----------|---------|----------------------------------------|
| id        | INTEGER | Auto-incremented primary key           |
| order_id  | TEXT    | Unique order identifier                |
| date      | TEXT    | Date of the transaction (YYYY-MM-DD)   |
| category  | TEXT    | Product category (e.g., Electronics)   |
| product   | TEXT    | Product name                           |
| region    | TEXT    | Sales region (e.g., East, North)       |
| quantity  | INTEGER | Number of units sold                   |
| price     | REAL    | Price per unit                         |

## 🧑‍💻 What the Scripts Do

### ✅ `create_sales_db.py`

- Creates a SQLite database (`sales_data.db`)
- Defines the `sales` table
- Inserts 20 rows of realistic superstore-style sales data

### ✅ `analyze_sales.py`

- Connects to the database
- Runs a SQL query to calculate total revenue per product
- Uses `pandas` to load query results
- Visualizes the result as a bar chart using `matplotlib`

## 📊 Example Output

![Product vs Revenue Bar Chart](product_vs_revenue.png)

## 🔧 Requirements

Make sure you have the following Python libraries installed:

```bash
pip install pandas matplotlib

SQLite is included with Python by default.

🧠 Learning Outcomes
Practice writing and running SQL queries in Python

Learn how to connect to SQLite using sqlite3

Aggregate data using GROUP BY

Visualize sales summaries using matplotlib

📌 Task Context
This project was submitted as part of the Data Analyst Internship Task 7, where the objective was to:

Create a tiny SQLite sales database

Query basic sales summaries (total revenue, quantity)

Display results using print and plots

📎 License
This project is open-source and free to use for learning purposes.
