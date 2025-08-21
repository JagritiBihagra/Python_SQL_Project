# Python_sql_E-Commerce Data Analytics Project

This project is an **E-commerce Data Analysis Project** built using **Python** and **SQL**.
It leverages multiple datasets to analyze sales, customers, and product performance, helping businesses make **data-driven decisions**.

---

##  Features

* **Data Cleaning & Preprocessing**
  * Handled missing values, duplicates, and inconsistent formats.
    
* **SQL Database Integration**
  * Designed relational database schema for products, customers, and orders.
  * Performed queries for insights on revenue, top-selling products, and customer behavior.

* **Python Analytics & Visualization**
  * Data analysis with **Pandas, NumPy**
  * Visualizations with **Matplotlib / Plotly / Seaborn**

* **Business Insights**
  * Sales trends over time
  * Customer segmentation
  * Revenue breakdown by category

---


## 🗄 Database Schema

**Tables Used:**

* **Customers** (customer\_id, name, location, signup\_date, …)
* **Products** (product\_id, category, price, stock, …)
* **Orders** (order\_id, customer\_id, product\_id, quantity, order\_date, …)
* **Payments** (payment\_id, order\_id, payment\_method, amount, …)
* **Geolocation**
* **order_items**
* **sellers**

---

##  Tech Stack

* **Languages**: Python, SQL
* **Python Libraries**: Pandas, NumPy, Matplotlib, Seaborn, SQLAlchemy
* **Database**: MySQL
* **Tools**: Jupyter Notebook


---

## 📊 Example Queries

* **Top 5 Customers by Revenue**

  ```sql
  SELECT c.customer_id, c.name, SUM(o.quantity * p.price) AS total_spent
  FROM orders o
  JOIN customers c ON o.customer_id = c.customer_id
  JOIN products p ON o.product_id = p.product_id
  GROUP BY c.customer_id, c.name
  ORDER BY total_spent DESC
  LIMIT 5;
  ```

* **Monthly Sales Trend**

  ```sql
  SELECT DATE_TRUNC('month', order_date) AS month, SUM(quantity * price) AS revenue
  FROM orders
  JOIN products ON orders.product_id = products.product_id
  GROUP BY month
  ORDER BY month;
  ```

---

## 📈 Sample Visualizations

* Sales trends over time
* Revenue by category
* Customer segmentation

*(Add screenshots of your plots here if possible)*

---


---

👉 Do you want me to also generate a **ready-to-use `requirements.txt`** (with common Python + SQL libraries), so you can include it in your repo?
