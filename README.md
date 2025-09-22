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

## 📂 Schema Description

The database schema includes the following tables:

products → Stores product details (SKU, name, price, stock quantity).
suppliers → Contains supplier information.
customers → Stores customer details.
orders → Tracks orders placed by customers.
order_items → Line items for each order (quantity, price, linked to products).
product_suppliers → Resolves the many-to-many relationship between products and suppliers.

## 🔑 Constraints & Relationships

PRIMARY KEY on every table (e.g., product_id, supplier_id, order_id).
FOREIGN KEY constraints for relationships:
orders.customer_id → customers.customer_id
order_items.order_id → orders.order_id
order_items.product_id → products.product_id
product_suppliers.product_id → products.product_id
product_suppliers.supplier_id → suppliers.supplier_id
NOT NULL constraints to enforce required fields.
UNIQUE constraint on products.sku to prevent duplicate product codes.

## ⚙️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Sammyojima/inventory-database-assignment.git
2. Open MySQL and log in:
    mysql -u root -p

3. Run the SQL script:
    SOURCE inventory_schema.sql;


## 📝 Notes

Designed and tested on MySQL 8.x.
Schema follows 1NF, 2NF, and 3NF to eliminate redundancy.
Can be extended with triggers, views, or stored procedures for advanced functionality.

## 📜 License

This project is for academic purposes. Feel free to use and adapt for learning.

👤 **Author**
Samuel Ojima Idakwo
