# SQL_Learning
## SQL Basics
## Day 1 

Suppose you have a table called **Employees**.


| EmployeeID | Name | Age | Salary |
| :---: | :--- | :---: | :---: |
| **1** | Alice | 25 | $40,000 |
| **2** | Bob | 30 | $50,000 |
| **3** | Charlie | 28 | $45,000 |


Q1:
Write an SQL query to display all columns and all rows from the Employees table.

🔵Query : SELECT * FROM Employees;

⭐Output:
| EmployeeID | Name | Age | Salary |
| :---: | :--- | :---: | :---: |
| **1** | Alice | 25 | $40,000 |
| **2** | Bob | 30 | $50,000 |
| **3** | Charlie | 28 | $45,000 |


Q2:
Write an SQL query to display only the Name and Salary columns from the Employees table.

🔵Query: SELECT Name, Salary FROM Employees;

⭐Output:
|  Name |  Salary |
|  :--- |  :---: |
|  Alice | $40,000 |
|  Bob | $50,000 |
|  Charlie | $45,000 |
