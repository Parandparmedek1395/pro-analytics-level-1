# SQL and Python Integration

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

A lot of data is very well structured - think employee records, sales, log files and more.
It may come from a relational database system which keeps information in tables (relations) that can be linked on matching columns, e.g. one table has your student record, and another has a record (row) for each course you've taken. A special language as been developed to work with these databases - SQL (Structured Query Language).
Knowing SQL basics will enable you to work effectively with your favorite AI assistant to generate the specific queries needed to gain insights from your data.

## Introduction

There are entire books written on SQL and you can spend a lifetime learning it.
You may need to use SQL when you interact directly with a database management system (DBMS) like MySQL, PostgreSQL, or Microsoft SQL Server.
With Python, you can also create and use file-based databases without any additional DBMS system.
We'll use this approach to learn SQL basics and some key professional practices.

## Recommendations

- Store SQL queries in separate `.sql` files.
- This keeps your code clean and easy to maintain.
- Use parameterized queries to prevent SQL injection attacks.
- Avoid concatenating strings to build SQL queries, especially if including user input.
- Manage database connections to ensure data integrity and efficient use of resources.
- Be aware of the potential dangers when using user input and always keep security in mind.

## Examples

```python
# Import the sqlite3 module from the Python standard library.
import sqlite3

# Create a connection to the database.
connection = sqlite3.connect('data.db')

# Create a cursor object to execute SQL queries.
cursor = connection.cursor()

# Read SQL from a file
# 'CREATE TABLE IF NOT EXISTS students (id INTEGER PRIMARY KEY, name TEXT, grade REAL)'
create_table_query = open('create_table.sql', 'r').read()

# Create a table.
cursor.execute(create_table_query)

# Insert a row of data.
# Shown for illustration only - these should be .sql files and used as shown above.
cursor.execute('INSERT INTO students VALUES (1, "Alice", 3.5)')
cursor.execute('INSERT INTO students VALUES (2, "Bob", 3.0)')
cursor.execute('INSERT INTO students VALUES (3, "Charlie", 3.8)')
cursor.execute('INSERT INTO students VALUES (4, "Denise", 4.0)')

# Find students where grade is greater than 3.5.
cursor.execute('SELECT * FROM students WHERE grade > 3.5')

# Find students where name like 'A%'.
cursor.execute('SELECT * FROM students WHERE name LIKE "A%"')

# Save (commit) the changes.
connection.commit()

# Close the connection.
connection.close()
```

## Resources

- [SQL Basics](https://www.w3schools.com/sql/sql_intro.asp)
- [xkcd Comic: Little Bobby (Drop) Tables](https://xkcd.com/327/)
- [SQL Injection](https://www.w3schools.com/sql/sql_injection.asp)
