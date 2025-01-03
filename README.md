# Northwind Database Schema

This repository contains a MySQL script that sets up the Northwind database schema. The Northwind database is a classic sample database used for demonstrating database concepts and practices. This schema includes tables for customers, employees, orders, products, and more, which can be useful for learning SQL and database management.

## Overview

The SQL script was generated by MySQL Workbench and includes the following features:

- **Schema Creation**: The script creates a schema named `northwind`.
- **Table Definitions**: It defines multiple tables, including:
  - `customers`
  - `employees`
  - `orders`
  - `products`
  - `suppliers`
  - `shippers`
  - `invoices`
  - And more...
  
- **Relationships**: The script establishes foreign key relationships between tables to maintain data integrity.

## Getting Started

To set up the Northwind database on your local MySQL server, follow these steps:

### Prerequisites

- MySQL Server installed on your machine.
- MySQL Workbench or any other MySQL client to execute the SQL script.

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/bsills1040/northwind-database.git
   cd northwind-database

2. **Open MySQL Workbench**:

  Launch MySQL Workbench and connect to your MySQL server.

3. **Execute the SQL Script**:
   Open the northwind.sql file in MySQL Workbench.
   Execute the script by clicking on the lightning bolt icon or pressing Ctrl + Shift + Enter.

4. **Verify the Setup**:
   After execution, you can verify that the tables have been created by running the following SQL command: SHOW TABLES IN northwind;

### Usage

Once the database is set up, you can start using it for various purposes, such as:

Running queries to retrieve data.
Inserting new records into the tables.
Performing joins to analyze relationships between different entities.

### Example Queries

Here are a few example queries you can run against the Northwind database:

**Retrieve all customers**: 

SELECT * FROM customers;

**Get orders placed by a specific customer**:

SELECT * FROM orders WHERE customer_id = 1;

**Count the number of products in each category**: 

SELECT category, COUNT(*) AS product_count
FROM products
GROUP BY category;

### Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request. Any improvements or additional features are welcome!

### License
This project is licensed under the MIT License - see the LICENSE file for details.

### Acknowledgments
This schema is based on the classic Northwind database, which is widely used for educational purposes in database management.

