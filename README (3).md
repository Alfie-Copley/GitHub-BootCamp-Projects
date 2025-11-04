# Database Concepts Workbook Summary

## Day 1: Task 1 – Database Fundamentals
Explored key database concepts and relationships:
- **Primary Key** – Uniquely identifies each record in a table; must be unique and non-null.
- **Secondary Key** – A candidate key not chosen as the primary; may allow duplicates or nulls.
- **Foreign Key** – Links one table to another by referencing the primary key, enforcing referential integrity.

### Real-world Relationship Examples
- **One-to-One:** Person ↔ Passport, Employee ↔ Company Car, Patient ↔ Medical Record  
- **One-to-Many:** Customer → Orders, Author → Books, Department → Employees  
- **Many-to-Many:** Students ↔ Courses, Movies ↔ Actors, Products ↔ Orders (via junction tables)

## Day 1: Task 2 – Relational vs Non-Relational Databases
### Relational Databases (RDBMS)
- Store data in structured tables with relationships defined by primary and foreign keys.
- Use SQL for queries (e.g., MySQL, PostgreSQL).

### Non-Relational Databases (NoSQL)
- Store unstructured or semi-structured data (documents, key-value, graph).
- More flexible and scalable, suited for social media, IoT, and large-scale real-time applications.

**Example:** E-commerce product catalogues benefit from NoSQL due to variable product attributes and scalability.

## Day 3: Task 1 – SQL JOIN Types
Explained six key join types and their uses:
- **Self Join:** Relates a table to itself (e.g., employees and managers).  
- **Inner Join:** Returns only matching rows from both tables (e.g., products with sales).  
- **Left Join:** All records from the left, and matching from the right (e.g., all customers, even without orders).  
- **Right Join:** All records from the right, matching from the left (e.g., all customers including those without orders).  
- **Full Join:** Combines all rows from both tables, showing nulls where no matches exist (e.g., all students and all library cards).  
- **Cross Join:** Combines every row with every row in another table (e.g., all colour and size combinations).

## Day 4: Task 1 – Database Design Essay
Designed a database for a small retail business to manage inventory, sales, and loyalty data.

### Key Steps
1. **Understanding Requirements:** Store data on inventory, sales, customers, and loyalty points.  
2. **Users:** Store owner and customers; owners need reports, customers view loyalty points.  
3. **Design:** Two main tables – inventory/sales data and customer information.  
4. **Implementation:** Created `Store_db` with SQL commands such as:  
   ```sql
   CREATE DATABASE Store_db;
   USE Store_db;
   CREATE TABLE DailySummary (
       SummaryDate DATE PRIMARY KEY,
       TotalCustomers INT,
       TotalProductsSold INT,
       TotalStockRemaining INT
   );
   INSERT INTO DailySummary (SummaryDate, TotalCustomers, TotalProductsSold, TotalStockRemaining)
   VALUES ('2025-09-29', 30, 150, 450);
   ```
5. **Maintenance:** Regular backups, accuracy checks, and data security measures.

## Day 4: Task 2 – SQL Practical Scenarios
Applied SQL queries to solve real-world data problems using the `world_db` dataset.

### Example Scenarios
- **Count Cities in USA** – Determine number of U.S. cities.  
- **Highest Life Expectancy** – Identify top country for longevity.  
- **Cities with ‘New’ in Name** – Compile list for marketing campaign.  
- **Population Queries** – Filter cities above 2M, between 500K–1M, or smallest populations.  
- **Sorting and Limiting Results** – Show first 10 cities, or rows 31–40 by population.  
- **Geographic Queries** – Find European cities, capital of Spain, and average population per country.  
- **Comparisons** – Capital city populations, high GDP per capita cities, and countries with low density.  

---
**Overall Focus:**  
Developed a comprehensive understanding of database structures, relationships, SQL joins, and practical data analysis.  
Learned how to design, implement, and query a functional database system using real-world scenarios.
