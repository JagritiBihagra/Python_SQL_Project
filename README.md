# Python_sql_E-Commerce Data Analytics Project

This project is an **E-commerce Data Analysis Project** built using **Python** and **SQL**.
It leverages multiple datasets to analyze sales, customers, and product performance, helping businesses make **data-driven decisions**.

---

##  Features

* **Data Cleaning & Preprocessing**
  * Handled missing values, duplicates, and inconsistent formats.
    
* **SQL Database Integration**
  * Designed relational database schema for the datasets used.
  * Performed queries for insights on revenue, top-selling products, and customer behavior.

* **Python Analytics & Visualization**
  * Data analysis with **Pandas, NumPy**
  * Visualizations with **Matplotlib and Seaborn**

* **Business Insights**
  * Sales trends over time
  * Customer segmentation
  * Revenue breakdown by category

---


## 🗄 Database Schema

**Tables Used:**

* **Customers** (customer_id, customer_unique_id, customer_zip_code_prefix, customer_city, customer_state)
* **Products** (product_id, product_category, product_name_length, product_description_length, product_photos_qty, product_weight_g, product_length_cm, product_height_cm, product_width_cm)
* **Orders** (order_id, customer_id, order_status, order_purchase_timestamp, order_approved_at, order_delivered_carrier_date, order_delivered_customer_date, order_estimated_delivery_date)
* **Payments** (order_id, payment_sequential, payment_type, payment_installments, payment_value)
* **Geolocation** (geolocation_zip_code_prefix, geolocation_lat, geolocation_lng, geolocation_city, geolocation_state)
* **order_items** (order_id, order_item_id, product_id, seller_id, shipping_limit_date, price, freight_value)
* **sellers** (seller_id, seller_zip_code_prefix, seller_city, seller_state)

---

##  Tech Stack

* **Languages**: Python, SQL
* **Python Libraries**: Pandas, NumPy, Matplotlib, Seaborn
* **Database**: MySQL
* **Tools**: Jupyter Notebook


---


---


---

👉 Do you want me to also generate a **ready-to-use `requirements.txt`** (with common Python + SQL libraries), so you can include it in your repo?
