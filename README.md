# SQL_Learning
## SQL Basics

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

Suppose you have a table called **Employees**.

| EmployeeID | Name | Age | Salary | Department|
| :---: | :--- | :---: | :---: | :---: |
| **1** | Alice | 25 | $40,000 |IT |
| **2** | Bob | 30 | $50,000 |HR|
| **3** | Charlie | 28 | $45,000 |IT|

Q3:
Write an SQL query to display all employees who work in the **IT** department.

🔵Query: SELECT * FROM Employees WHERE Department = 'IT';

⭐Output:
| EmployeeID | Name | Age | Salary | Department|
| :---: | :--- | :---: | :---: | :---: |
| **1** | Alice | 25 | $40,000 |IT |
| **3** | Charlie | 28 | $45,000 |IT|

