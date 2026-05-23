# Brewbean's SQL Database Project

## Overview
This project provides hands-on practice using SQL with the Brewbean’s database in Oracle SQL Developer. The assignment focuses on learning how to run database setup scripts, work with relational database tables, and create SQL queries to retrieve and organize data.

The project also demonstrates an understanding of relational database concepts such as:
- Primary keys
- Foreign keys
- Table relationships
- Data integrity
- Querying and filtering data
- Joining multiple tables

The assignment includes work with both the Brewbean’s (BB) database and the Moviemania database schema.

---

# Objectives
- Execute SQL setup scripts in Oracle SQL Developer
- Verify table schemas and relationships
- Practice writing SELECT statements
- Use aggregate functions such as SUM
- Perform INNER JOIN operations
- Compare ANSI joins with traditional joins
- Create and modify tables
- Insert, update, rollback, and commit data changes
- Understand checkout logic and database workflow concepts

---

# Database Scripts

## Brewbean’s Database (`c1_BBcreate.sql`)
The `c1_BBcreate.sql` script creates the core Brewbean’s database structure. It defines tables, relationships, primary keys, foreign keys, and inserts initial data required for the database system to function properly.

The schema supports:
- Product management
- Customer baskets
- Orders
- Product options
- Shopper information

---

## Moviemania Database (`c1_MMcreate.sql`)
The `c1_MMcreate.sql` file defines a movie rental database schema. It creates tables for:
- Members
- Movies
- Rentals
- Payment methods

The script also establishes relationships between tables to maintain relational integrity and support accurate transaction tracking.

---

# Query Tasks and Results

## Confirming Table Schemas
This section demonstrates successful creation of the BB database tables and verifies that the schema was built correctly with all required constraints and relationships.

---

## Product Option JOIN Query
This query joins:
- `bb_product`
- `bb_productoption`
- `bb_productoptiondetail`
- `bb_productoptioncategory`

The query retrieves detailed product configuration information using INNER JOIN operations and confirms that relational data is being returned correctly.

### Example Concepts Demonstrated
- Multi-table joins
- Foreign key relationships
- Data retrieval across related tables

---

## DISTINCT Product Query
This query retrieves a unique list of product IDs sold from the `bb_basketItem` table using the `DISTINCT` keyword.

### SQL Concepts Used
- DISTINCT
- ORDER BY
- Data filtering

---

## February 2012 Orders Query
This query retrieves all orders placed during February 2012 from the `bb_basket` table and formats the date using the `TO_CHAR` function.

### SQL Concepts Used
- Date filtering
- TO_CHAR formatting
- WHERE clause conditions

---

## Total Quantity Sold Query
This query calculates the total quantity sold for each product using:
- `SUM`
- `GROUP BY`

The results help analyze sales totals across all products.

---

## ANSI JOIN vs Traditional JOIN
Two versions of the same query were written:
1. ANSI JOIN syntax
2. Traditional join syntax

Both queries return:
- Basket ID
- Product ID
- Product name
- Product description

This demonstrates multiple valid approaches for joining related tables in SQL.

---

## Customer Information JOIN Query
This query extends previous joins by including shopper information from the `bb_shopper` table.

The final result displays:
- Basket ID
- Product ID
- Product name
- Product description
- Shopper last name

---

# Additional Assignments

## Assignment 1-2 — Third-Party PL/SQL Tool Review

### Toad for Oracle
One popular third-party PL/SQL development tool is **Toad for Oracle** by Quest Software.

### Useful Features
#### 1. Code Editor with Auto-Completion
Provides intelligent SQL and PL/SQL suggestions for:
- Table names
- Column names
- SQL syntax

This helps reduce syntax errors and improves development speed.

#### 2. Schema Browser
Allows developers to visually inspect:
- Tables
- Indexes
- Procedures
- Constraints

without manually writing SQL queries.

---

## Assignment 1-3 — Brewbean’s Checkout Logic

When the checkout button is clicked, the system would logically perform the following steps:

1. Retrieve all items from the customer basket
2. Calculate the subtotal
3. Determine shipping costs
4. Identify the customer billing state
5. Retrieve applicable tax rates
6. Calculate tax amounts
7. Compute the final order total
8. Display the final checkout summary

This process demonstrates how databases support real-world e-commerce functionality.

---

# Technologies Used
- Oracle SQL Developer
- SQL
- Relational Databases
- PL/SQL Concepts

---

# Screenshots
All screenshots demonstrating query execution and results are stored in the `/screenshots` folder.

---

# Author
Zion Adedipe

Purdue University — CIT Coursework
