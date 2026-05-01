# Global Demographic Analysis (SQL) 🗄️⚡

## 📌 Project Overview
This project involves extracting actionable insights from a relational database containing over 4,000 cities and 200+ countries. I used **MySQL** to perform complex queries that solve real-world scenarios, such as urban planning, economic research, and demographic analysis.

## 🛠 Tech Stack
- **Language:** SQL 
- **Tool:** MySQL Workbench
- **Key Concepts:** Joins, Subqueries, Aggregations (AVG, COUNT), and Pagination (LIMIT/OFFSET).

## ⚙️ Key Technical Features
- **Relational Data Mapping:** Performed `INNER JOINs` between the `City` and `Country` tables to link local demographics with national metadata.
- **Economic Benchmarking:** Implemented **Subqueries** to filter countries with above-average GNP, identifying top-performing global economies.
- **Advanced Filtering:** Used `LIKE` operators and `BETWEEN` clauses for targeted string and numerical search patterns.
- **Data Summarization:** Leveraged `GROUP BY` and `ORDER BY` to create ranked reports for executive decision-making.

## 📖 Query Samples & Results
### 1. Identifying National Capitals
*Connecting the country table to the city table to find specific capital names.*
```sql
SELECT ci.Name AS Capital_Name FROM country c JOIN city ci ON c.Capital = ci.ID WHERE c.Name = 'Spain';
