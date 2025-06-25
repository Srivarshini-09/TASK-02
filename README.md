# 🧾 SQL Developer Internship – Task 2

## 📌 Task Title: Data Insertion and Handling Nulls

This project is part of the **SQL Developer Internship** and focuses on using Data Manipulation Language (DML) to insert, update, delete records, and handle `NULL` values effectively within an e-commerce database.

---

## 🧠 Objective

Practice the following SQL operations:
- Insert data using `INSERT INTO`
- Update records using `UPDATE`
- Delete records using `DELETE`
- Handle missing values using `NULL`
- Query data using conditions like `IS NULL`

---

## 🛠️ Tools & Environment

- **SQL Dialect:** MySQL  
- **Platform:** MySQL Workbench  
- **Database Used:** `ECommerceDB`

---

## 📂 What's Included

The SQL file (`task2_insertion.sql`) performs the following:

### ✅ Data Insertion
- Added sample data into tables: `Category`, `Product`, `Customer`, `Orders`, `OrderItem`, and `Payment`.
- Handled optional fields using `NULL` where applicable.

### 🛠 Data Updates
- Updated customer contact information.
- Adjusted product stock after orders.
- Modified payment method details.

### ❌ Data Deletion
- Deleted a customer with no orders.
- Deleted a specific order using `OrderID`.

### 🧪 Null Handling
- Inserted customers with missing values (`NULL` for phone and address).
- Queried customers with missing phone numbers using `IS NULL`.

---

## 🧱 Reference: Task 1 – Database Schema Setup

> *Note: This project builds upon the database schema created in Task 1.*

In **[Task 1](https://github.com/Srivarshini-09/Task-01.git)**, the foundational database schema was implemented with the following tables:
- `Category`
- `Product`
- `Customer`
- `Orders`
- `OrderItem`
- `Payment`

Key features included:
- Auto-incrementing primary keys  
- Foreign key constraints with `ON DELETE CASCADE` and `ON UPDATE CASCADE`  
- Default values (e.g., `OrderDate`, `Stock`)  
- Support for optional fields like `Phone`, `Address`, and `Description`

This schema supports all data operations performed in Task 2.

---

## 🧪 How to Run the Project

1. Set up the `ECommerceDB` database using Task 1: [View Schema](https://github.com/Srivarshini-09/Task-01.git)
2. Open your SQL environment (DB Fiddle, MySQL Workbench, etc.)
3. Paste and run the SQL from `task2_insertion.sql`.
4. Use the following queries to verify results:
```sql
SELECT * FROM Customer;
SELECT * FROM Orders;
SELECT * FROM Product;
SELECT * FROM Payment;
SELECT * FROM Customer WHERE Phone IS NULL;
