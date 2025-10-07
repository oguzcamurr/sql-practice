#SQL Practice by Oğuz Çamur

🗄️ This repository contains my SQL practice queries and case studies.  
I use **MySQL Workbench** on Windows to build and test queries with sample datasets.  

---

## 📂 Structure
- **basic/** → SELECT, WHERE, ORDER BY, LIMIT  
- **intermediate/** → JOIN, GROUP BY, HAVING  
- **advanced/** → Window Functions (RANK, ROW_NUMBER, QUALIFY, etc.)  
- **datasets/** → CSV or sample databases (e.g. Olist, Chinook, Sakila)  
- **queries/** → Real business-style questions (top customers, monthly growth, retention)

---

## 🛠️ Setup
1. Install [MySQL Community Edition](https://dev.mysql.com/downloads/installer/).  
2. Clone this repo:  
   ```bash
   git clone https://github.com/oguzcamurr/sql-practice.git
   ```
   
Run queries in MySQL Workbench:
```bash
USE testdb;
SOURCE queries/top_customers.sql;
```

📊 Example Queries
Create Database & Table
```bash
CREATE DATABASE testdb;
USE testdb;

CREATE TABLE customers (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50),
    city VARCHAR(50),
    spend DECIMAL(10,2)
);
```

Insert Sample Data
```bash
INSERT INTO customers (name, city, spend)
VALUES
('Ali', 'Istanbul', 120.50),
('Ayşe', 'Ankara', 300.00),
('Mehmet', 'Izmir', 50.75);
```
Get All Customers
```bash
SELECT * FROM customers;
```
🎯 Goals
Practice SQL daily (from basics to advanced window functions)

Apply queries on real-world datasets (Kaggle, sample DBs)

Document queries for data analytics & business case studies

Build a public SQL portfolio to showcase my skills

👨‍💻 Author: Oğuz Çamur
📬 Reach me on [LinkedIn](https://www.linkedin.com/in/oguzcamur) | [GitHub](https://github.com/oguzcamurr)
