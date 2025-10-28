# 🚀 My Data Engineering SQL Portfolio

Welcome to my personal SQL portfolio. This repository is a living collection of my work, designed to practice and showcase my proficiency in the SQL skills essential for data engineering.

## 🚧 How This Repository is Structured

This portfolio is organized into folders, each corresponding to a core SQL concept. Inside each folder, you'll find `.sql` files with my solutions to various problems, demonstrating that concept in action.

---

## 📚 Core SQL Concepts for Data Engineering

### 01. 💡 SQL Basics & Querying

*The fundamental building blocks for retrieving and filtering data.*

* `SELECT` / `FROM` / `WHERE`
* `ORDER BY`
* `LIMIT` / `TOP`
* `DISTINCT`
* `AS` (Aliasing)
* Logical Operators (`AND`, `OR`, `NOT`, `IN`, `BETWEEN`, `LIKE`)
* `NULL` Handling (`IS NULL`, `IS NOT NULL`, `COALESCE`)

### 02. 🏛️ Data Definition Language (DDL)

*Commands for building and managing the database's structure.*

* `CREATE TABLE`
* Data Types (e.g., `VARCHAR`, `INT`, `TIMESTAMP`)
* Constraints (`PRIMARY KEY`, `FOREIGN KEY`, `UNIQUE`, `NOT NULL`, `CHECK`)
* `ALTER TABLE`
* `DROP TABLE` & `TRUNCATE TABLE`
* `CREATE VIEW` / `DROP VIEW`

### 03. ✏️ Data Manipulation Language (DML)

*Commands for interacting with the data inside the tables.*

* `INSERT INTO`
* `UPDATE`
* `DELETE`

### 04. 📊 Aggregations & Grouping

*Summarizing data to find insights.*

* `GROUP BY`
* Aggregate Functions: `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`
* `HAVING` (Filtering groups)

### 05. 🔗 Joins & Unions

*The core of relational SQL: combining data from multiple tables.*

* `INNER JOIN`
* `LEFT JOIN` / `RIGHT JOIN`
* `FULL OUTER JOIN`
* `CROSS JOIN`
* `UNION` / `UNION ALL`
* `INTERSECT` / `EXCEPT`

### 06.  nesting.md Subqueries & CTEs

*Techniques for breaking down complex problems into logical, readable steps.*

* **Subqueries:**
    * In `WHERE` clauses (e.g., `... WHERE col IN (SELECT ...)`).
    * In `FROM` clauses (Derived Tables).
    * In `SELECT` clauses (Scalar Subqueries).
* **Common Table Expressions (CTEs):**
    * `WITH ... AS (...)`
    * Recursive CTEs (for hierarchical data)

### 07. 🖼️ Window Functions

*Performing calculations across sets of rows, without collapsing them.*

* `PARTITION BY` (Defining the "window")
* **Ranking:** `ROW_NUMBER()`, `RANK()`, `DENSE_RANK()`
* **Analytic:** `LAG()`, `LEAD()`
* **Aggregate:** `SUM() OVER (...)`, `AVG() OVER (...)` (e.g., for running totals)

### 08. 🛠️ Advanced Functions & Operations

*Tools for complex data cleaning, transformation, and conditional logic.*

* **Conditional Logic:** `CASE ... WHEN ... THEN ... END`
* **Pivoting:** `PIVOT` / `UNPIVOT` or using `CASE` statements
* **Date/Time:** `EXTRACT()`, `DATE_TRUNC()`, `INTERVAL`
* **String:** `CONCAT()`, `SUBSTRING()`, `TRIM()`, `REPLACE()`
* **Type Casting:** `CAST(...)` or `::`

### 09. 🎛️ Procedural SQL & Automation

*Writing programmatic logic (scripts, functions, and procedures) in SQL.*

* `CREATE PROCEDURE` (Stored Procedures)
* `CREATE FUNCTION` (User-Defined Functions - UDFs)
* Variables, loops, and control flow (e.g., `IF`/`ELSE`)

### 10. ⚡ Performance & Optimization

*Understanding *how* queries run and making them faster and more efficient.*

* **Indexing:** `CREATE INDEX`, B-Tree, Clustered vs. Non-Clustered
* **Query Planning:** `EXPLAIN` / `EXPLAIN ANALYZE`
* **Table Partitioning:** Strategies for splitting large tables
* **Materialized Views:** Pre-calculating results
* Query Anti-Patterns (and how to fix them)

### 11. 🔒 Transactions & Data Control

*Ensuring data integrity, consistency, and security.*

* `BEGIN`, `COMMIT`, `ROLLBACK` (Transaction Control)
* `GRANT` / `REVOKE` (Permissions)
* Isolation Levels
