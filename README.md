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

Q4:
Write an SQL query to display only the Name and Department of all employees.

🔵Query: SELECT Name, Department FROM Employees;

⭐Output:
| Name  | Department|
| :---: | :---: | 
|  Alice  | IT |
|  Bob  |HR|
|  Charlie  |IT|

Suppose you have a table called **Employees**.
| EmployeeID | Name    | Age | Department | Salary |
| ---------- | ------- | --- | ---------- | ------ |
| 1          | Alice   | 25  | HR         | 40000  |
| 2          | Bob     | 30  | IT         | 50000  |
| 3          | Charlie | 28  | Finance    | 45000  |
| 4          | David   | 35  | IT         | 60000  |
| 5          | Eva     | 27  | HR         | 42000  |
| 6          | Frank   | 32  | IT         | 55000  |

Q5:
Write an SQL query to display all the salaries of employees who are above 45000.


🔵Query:
SELECT * FROM Employees
WHERE Salary > 45000;

⭐Output:
| EmployeeID | Name  | Age | Department | Salary |
| ---------- | ----- | --- | ---------- | ------ |
| 2          | Bob   | 30  | IT         | 50000  |
| 4          | David | 35  | IT         | 60000  |
| 6          | Frank | 32  | IT         | 55000  |


Suppose you have a table called **Employees**.
| EmployeeID | Name    | Age | Department | Salary |
| ---------- | ------- | --- | ---------- | ------ |
| 1          | Alice   | 25  | HR         | 40000  |
| 2          | Bob     | 30  | IT         | 50000  |
| 3          | Charlie | 28  | Finance    | 45000  |
| 4          | David   | 35  | IT         | 60000  |
| 5          | Eva     | 27  | HR         | 42000  |
| 6          | Frank   | 32  | IT         | 55000  |


Q6:
Write an SQL query to display all employees whose age is less than 30.

🔵Query:
SELECT * FROM Employees WHERE Age < 30;

⭐Output:
| EmployeeID | Name    | Age | Department | Salary |
| ---------- | ------- | --- | ---------- | ------ |
| 1          | Alice   | 25  | HR         | 40000  |
| 3          | Charlie | 28  | Finance    | 45000  |
| 5          | Eva     | 27  | HR         | 42000  |





