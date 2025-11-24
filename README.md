# Task 7 – Sales Data Analysis Using Python and SQLite

This project demonstrates how to connect Python with SQLite, perform SQL queries, analyze sales data, and visualize results using Pandas and Matplotlib.

---

## 📁 Files Included

| File Name | Purpose |
|-----------|---------|
| create_db.py | Creates the SQLite database with a `sales` table and sample data |
| sales_data.db | SQLite database file containing the sales data |
| task7_analysis.py | Python script to query the database, calculate total revenue, and generate visualization |
| sales_revenue_chart.png | Bar chart showing revenue by product |
| README.md | Documentation file explaining the project |
| (Optional) screenshot.png | Displays program output |

---

## ⚙️ How to Run the Project

### ▶️ Step 1: Create the Database  
Run the file below to generate `sales_data.db`:


---

### ▶️ Step 2: Run the Analysis and Visualization  
Execute the analysis script:


This will:
✔ Display total quantity and revenue per product  
✔ Generate and save `sales_revenue_chart.png`  

---

## 📊 SQL Query Used

```sql
SELECT 
    product,
    SUM(quantity) AS total_quantity,
    SUM(quantity * price) AS total_revenue
FROM sales
GROUP BY product
ORDER BY total_revenue DESC;

This will:
✔ Display total quantity and revenue per product  
✔ Generate `sales_revenue_chart.png`

---


## 📊 Output Example

The analysis prints data like this:

| Product | Total Quantity | Total Revenue |
|---------|---------------|---------------|
| Product A | 17 | 850 |
| Product C | 7 | 1050 |
| Product B | 7 | 700 |

And creates this chart:  
📎 `sales_revenue_chart.png`

---

## 🎯 Project Learning Outcomes

✔ Working with SQLite in Python  
✔ Executing SQL `GROUP BY` and aggregate functions  
✔ Using Pandas to convert SQL results into DataFrame  
✔ Plotting bar chart using Matplotlib  
✔ Saving and documenting project for GitHub submission

---

