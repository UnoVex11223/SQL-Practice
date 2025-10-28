# My Data Engineering SQL Portfolio

This repository is my personal collection of SQL queries, problems, and concepts, specifically focused on the skills required for **Data Engineering**. It serves as a living library of my solutions and a structured way to practice and demonstrate my SQL proficiency.

## 🚧 How This Portfolio is Structured

This repository is organized into folders, each corresponding to a core SQL concept listed below. Inside each folder, you'll find `.sql` files demonstrating the concept, often using example problems (e.g., LeetCode, HackerRank, or custom scenarios).

## 🗂️ SQL Concepts for Data Engineering

### 01-SQL-Basics-and-Querying

Covers the fundamental building blocks of querying data.

* `SELECT` / `FROM` / `WHERE`: The foundation of all queries.
* `ORDER BY`: Sorting results.
* `LIMIT` / `TOP`: Restricting the number of rows returned.
* `AS`: Aliasing columns and tables.
* `DISTINCT`: Finding unique values.
* Operators: `AND`, `OR`, `NOT`, `IN`, `BETWEEN`, `LIKE`.
* `NULL` Handling: `IS NULL`, `IS NOT NULL`, `COALESCE`.

### 02-Data-Definition-Language-(DDL)

The commands used to define and manage database structures.

* `CREATE TABLE`: Defining new tables, data types, and constraints.
* Constraints: `PRIMARY KEY`, `FOREIGN KEY`, `UNIQUE`, `NOT NULL`, `CHECK`.
* `ALTER TABLE`: Modifying existing tables (adding columns, changing data types).
* `DROP TABLE`: Deleting tables.
* `TRUNCATE TABLE`: Emptying tables.
* `CREATE VIEW` / `DROP VIEW`: Creating virtual tables.

### 03-Data-Manipulation-Language-(DML)

The commands used for adding, removing, and changing data within tables.

* `INSERT INTO`: Adding new rows.
* `UPDATE`: Modifying existing rows.
* `DELETE`: Removing rows.

### 04-Aggregations-and-Grouping

Essential for summarizing and reporting on data.

* `GROUP BY`: Grouping rows that have the same values.
* Aggregate Functions: `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`.
* `HAVING`: Filtering data *after* aggregation.

### 05-Joins-and-Unions

The core of relational databases: combining data from multiple tables.

* `INNER JOIN`: Returning only matching rows from both tables.
* `LEFT JOIN`: Returning all rows from the left table, and matched rows from the right.
* `RIGHT JOIN`: Returning all rows from the right table, and matched rows from the left.
* `FULL OUTER JOIN`: Returning all rows when there is a match in either table.
* `CROSS JOIN`: Returning the Cartesian product of two tables.
* `UNION` / `UNION ALL`: Stacking results from multiple queries.
* `INTERSECT` / `EXCEPT`: Finding common or different rows between queries.

### 06-Subqueries-and-CTEs

Advanced techniques for breaking down complex problems.

* **Subqueries:** Queries nested inside other queries.
    * In `WHERE` clauses (e.g., `... WHERE column IN (SELECT ...)`).
    * In `FROM` clauses (Derived Tables).
    * In `SELECT` clauses (Scalar Subqueries).
* **Common Table Expressions (CTEs):**
    * `WITH ... AS (...)`: Defining temporary, named result sets for cleaner, more readable queries.
    * Recursive CTEs: Queries that reference themselves (e.g., for hierarchical data).

### 07-Window-Functions

The most powerful tool for complex analysis without self-joins.

* `PARTITION BY`: Defining the "window" or group of rows to operate on.
* **Ranking Functions:**
    * `ROW_NUMBER()`: Unique sequential number for each row.
    * `RANK()`: Rank with gaps for ties.
    * `DENSE_RANK()`: Rank without gaps for ties.
* **Analytic Functions:**
    * `LAG()` / `LEAD()`: Accessing data from preceding or following rows.
* **Aggregate Window Functions:**
    * `SUM(...) OVER (...)`: Calculating running totals.
    * `AVG(...) OVER (...)`: Calculating moving averages.

### 08-Advanced-Functions-and-Operations

Useful functions for data cleaning, transformation, and manipulation.

* **Conditional Logic:**
    * `CASE ... WHEN ... THEN ... END`: Implementing if/then logic in SQL.
* **Pivoting:**
    * `PIVOT` / `UNPIVOT`: (SQL Server)
    * `CASE` statement pivoting: (The traditional, cross-database method).
* **Date/Time Functions:**
    * `EXTRACT()`, `DATE_PART()`: Getting parts of a date (day, month, year).
    * `DATE_TRUNC()`: Truncating dates to a specific precision.
    * `INTERVAL`: Performing date arithmetic.
* **String Functions:**
    * `CONCAT()`, `||`: Combining strings.
    * `SUBSTRING()`, `LEFT()`, `RIGHT()`: Extracting parts of a string.
    * `TRIM()`, `LOWER()`, `UPPER()`: Cleaning strings.
    * `REPLACE()`: Replacing parts of a string.
* **Casting:**
    * `CAST(...)` or `::`: Converting data types.

### 09-Procedural-SQL-and-Automation

Writing programmatic logic that lives in the database.

* `CREATE PROCEDURE`: Stored Procedures for encapsulating multi-step logic.
* `CREATE FUNCTION`: User-Defined Functions (UDFs) for reusable transformations.
* Variables, loops, and control flow (e.g., `IF`/`ELSE`, `WHILE` in T-SQL or PL/pgSQL).

### 10-Performance-and-Optimization

Writing queries that run efficiently is a critical DE skill.

* **Indexing:**
    * `CREATE INDEX`: How, when, and what to index.
    * Index Types: B-Tree, Clustered vs. Non-Clustered.
* **Query Planning:**
    * `EXPLAIN` / `EXPLAIN ANALYZE`: Reading and understanding query plans.
* **Table Partitioning:** Strategies for splitting large tables for performance.
* **Materialized Views:** Pre-calculating and storing query results.
* Query Anti-Patterns: Identifying and fixing inefficient queries (e.g., `SELECT *`, correlated subqueries).

### 12-Transactions-and-Data-Control

Ensuring data integrity and managing permissions.

* `BEGIN`, `COMMIT`, `ROLLBACK`: Transaction control for data integrity.
* `GRANT` / `REVOKE`: User permissions and access control.
* Isolation Levels: Understanding how transactions interact.
