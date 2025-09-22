# Inventory Database Schema

## 📌 Project Overview
This project is part of my Database Assignment.  
It contains a relational database schema for an **Inventory Management System**, designed using MySQL.

The schema defines tables, relationships, and constraints needed to manage inventory, suppliers, customers, and orders.

---

## 🗄️ Database Schema
The database contains the following tables:
- **Suppliers** → Stores supplier details.
- **Products** → Contains product information and stock.
- **Customers** → Stores customer details.
- **Orders** → Tracks customer orders.
- **Order_Items** → Links products to orders (Many-to-Many).

---

## ⚙️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Sammyojima/inventory-database-assignment.git
2. Open MySQL and log in:

    mysql -u root -p

3. Run the SQL script:

    SOURCE inventory_schema.sql;


**Verify the database:**

SHOW DATABASES;
USE inventory_db;
SHOW TABLES;

📝 **Notes**
This schema can be extended with more tables (e.g., Payments, Categories).
All tables use PRIMARY KEY, FOREIGN KEY, and constraints for data integrity.

👤 **Author**
Samuel Ojima Idakwo
