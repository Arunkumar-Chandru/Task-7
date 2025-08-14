# Java JDBC Employee Database App

## Overview
This is a simple **Java console application** that connects to a **MySQL database** using **JDBC** and performs **CRUD operations** on an `employees` table.  
The app allows you to **Add, View, Update, and Delete** employee records.

---

## Tools & Technologies
- **Java** (JDK 8+)
- **MySQL** (or PostgreSQL with minor changes)
- **JDBC Driver** (`mysql-connector-java`)
- **VS Code** (or any Java IDE)

---

## Database Setup (MySQL)

Run the following SQL queries in **MySQL Workbench** or **MySQL CLI**:

```sql
-- Create database
CREATE DATABASE employee_db;

-- Use database
USE employee_db;

-- Create employees table
CREATE TABLE employees (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    position VARCHAR(100),
    salary DECIMAL(10,2)
);
