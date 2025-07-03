# task-7-sales-summary-sqlite-python
TASK 7 - Sales Summary Using SQLite and Python (Data Analyst Internship)


# TASK 7 - Sales Summary Using SQLite and Python (Data Analyst Internship)

## 📋 Task Objective:
In this task, we analyze sales data stored in an SQLite database using Python.
We perform basic data analysis and create a revenue-based bar chart using SQL queries and visualization libraries.

---

## 🛠️ Tools Used:
- **Python** (with `sqlite3`, `pandas`, `matplotlib`)
- **SQLite** (Built-in with Python, no installation required)
- **Jupyter Notebook / Python Script**

---

## 📊 Key Steps Performed:
1. **SQLite Database Creation:**  
   - Created `sales_data.db` and `sales` table.
   - Inserted sample sales data (product, quantity, price).

2. **SQL Querying:**  
   - Retrieved total quantity sold and revenue per product using SQL:
```sql
SELECT product, SUM(quantity) AS total_qty, SUM(quantity * price) AS revenue 
FROM sales 
GROUP BY product;
