# 🚀 SQL Practice

Welcome to **SQL Practice**! This repository contains a collection of SQL queries and exercises designed to improve your SQL skills using the **Chinook SQLite database**. These queries cover various SQL concepts such as aggregation, joins, window functions, and data retrieval techniques.

## 📁 Project Structure

📌 **Week1.sql** → SQL queries for Week 1, including data retrieval, joins, and window functions

📌 **Chinook_Sqlite.sqlite** → Sample SQLite database used for query execution  


## 📊 Dataset Used: Chinook SQLite Database
The **Chinook database** is a sample database representing a digital media store. It contains tables such as **Customers, Invoices, Tracks, Artists, Albums, and Employees**, making it ideal for practicing SQL queries.

## ⚡ Getting Started
Follow these steps to set up and run SQL queries:

### 🔹 1. Clone the Repository
```bash
git clone https://github.com/PreethiVantala/SQL_Practice.git
cd SQL_Practice
```

### 🔹 2. Install SQLite
If you don’t have SQLite installed, install it using:
- **Ubuntu/Debian:** `sudo apt install sqlite3`
- **MacOS (Homebrew):** `brew install sqlite`
- **Windows:** Download SQLite from [sqlite.org](https://www.sqlite.org/download.html)

### 🔹 3. Run SQL Queries
#### **Option 1: Using SQLite CLI**
```bash
sqlite3 Chinook_Sqlite.sqlite < Week1.sql
```

#### **Option 2: Using Python**
Run the queries using Python and Pandas:
```python
import sqlite3
import pandas as pd

conn = sqlite3.connect("Chinook_Sqlite.sqlite")
query = "SELECT * FROM Customer LIMIT 5;"
df = pd.read_sql_query(query, conn)
print(df)
conn.close()
```

## 🛠️ SQL Concepts Practiced
✅ Aggregations (`SUM`, `COUNT`, `AVG`)
✅ Joins (`INNER JOIN`, `LEFT JOIN`)
✅ Window Functions (`OVER`, `PARTITION BY`)
✅ Filtering (`WHERE`, `LIKE`)
✅ Sorting (`ORDER BY`)
✅ Grouping (`GROUP BY`, `HAVING`)

## 🤝 Contributing
🎯 Contributions are welcome! If you have additional SQL queries or improvements, feel free to open an issue or submit a pull request.

## 🎉 Acknowledgments
Special thanks to the open-source community for providing the **Chinook SQLite database** and resources for SQL practice. 🚀

Happy querying! 😊



