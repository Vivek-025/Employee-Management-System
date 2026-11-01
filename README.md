# Employee Management System

A menu-based Python program that manages employee data stored in a MySQL database.

## Features

1. Add employee
2. View all employees
3. Search employee by name
4. Update salary
5. Delete employee (with confirmation)
6. Summary (total, average, min, max salary, city-wise count)

## Tech Stack

- Python
- MySQL
- mysql-connector-python
- python-dotenv
- Jupyter Notebook

## Database Setup

```sql
CREATE DATABASE company_db;
USE company_db;

CREATE TABLE emp (
    id INT PRIMARY KEY,
    name VARCHAR(30),
    city VARCHAR(30),
    salary FLOAT
);
```

## How to Run

1. Install the libraries:

```
   pip install mysql-connector-python python-dotenv
```

2. Copy `.env.example` to a new file named `.env` and put your own MySQL password in it:

```
   DB_HOST=localhost
   DB_USER=root
   DB_PASSWORD=your_password_here
   DB_NAME=company_db
```

3. Open `Mysql Python Connectivity.ipynb` in Jupyter and run the cell.

## Menu Preview

```
===== Employee Management System =====
1. Add employee
2. View all employees
3. Search employee
4. Update salary
5. Delete employee
6. Summary
7. Exit
```

## Concepts Used

- Database connection and cursor
- `commit` and `rollback`
- `try / except` error handling
- Aggregate functions and `GROUP BY`
- Environment variables to keep the password out of the code

## Author

Vivek
