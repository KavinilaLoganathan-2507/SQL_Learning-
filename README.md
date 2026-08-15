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
Write an SQL query to display  all Employees Sorted by age in ascending order 

🔵Query:
SELECT * FROM Employees
ORDER BY Age ASC;

⭐Output:
| EmployeeID | Name    | Age | Department | Salary |
| ---------- | ------- | --- | ---------- | ------ |
| 1          | Alice   | 25  | HR         | 40000  |
| 5          | Eva     | 27  | HR         | 42000  |
| 3          | Charlie | 28  | Finance    | 45000  |
| 2          | Bob     | 30  | IT         | 50000  |
| 6          | Frank   | 32  | IT         | 55000  |
| 4          | David   | 35  | IT         | 60000  |


Suppose you have a table called **Employees**.

| EmployeeID | Name    | Department |
| ---------- | ------- | ---------- |
| 1          | Alice   | HR         |
| 2          | Bob     | IT         |
| 3          | Charlie | Finance    |
| 4          | David   | IT         |
| 5          | Eva     | HR         |
| 6          | Frank   | IT         |


Q7:
Write a query to display all unique department names from the table 


🔵Query:
SELECT DISTINCT Department
FROM Employees;

⭐Output:
| Department |
| ---------- |
| HR         |
| IT         |
| Finance    |


Use this Employees table:
| EmployeeID | Name    | Department | Salary |
| ---------: | ------- | ---------- | -----: |
|          1 | Alice   | HR         |  40000 |
|          2 | Bob     | IT         |  50000 |
|          3 | Charlie | Finance    |  45000 |
|          4 | David   | IT         |  60000 |
|          5 | Eva     | HR         |  42000 |
|          6 | Frank   | IT         |  55000 |

Q8:
Write an SQL query to display the Name and Salary of employees whose salary is between 45000 and 55000, inclusive.

🔵Query:
SELECT Name, Salary
FROM Employees
WHERE Salary BETWEEN 45000 AND 55000;

⭐Output:
| Name    | Salary |
| ------- | -----: |
| Bob     | 50,000 |
| Charlie | 45,000 |
| Frank   | 55,000 |

Use this table for Employees:
| EmployeeID | Name    | Department | Salary |
| ---------: | ------- | ---------- | -----: |
|          1 | Alice   | HR         |  40000 |
|          2 | Bob     | IT         |  50000 |
|          3 | Charlie | Finance    |  45000 |
|          4 | David   | IT         |  60000 |
|          5 | Eva     | HR         |  42000 |
|          6 | Frank   | IT         |  55000 |

Q9:
Write an SQL query to display the Name and Department of employees who work in either the IT or HR department.

🔵Query:
SELECT Name, Department FROM Employees WHERE Department IN ('IT', 'HR');

⭐Output:
| Name  | Department |
| ----- | ---------- |
| Alice | HR         |
| Bob   | IT         |
| David | IT         |
| Eva   | HR         |
| Frank | IT         |



Use this table for Employees:
| EmployeeID | Name    | Department | Salary |
| ---------: | ------- | ---------- | -----: |
|          1 | Alice   | HR         |  40000 |
|          2 | Bob     | IT         |  50000 |
|          3 | Charlie | Finance    |  45000 |
|          4 | David   | IT         |  60000 |
|          5 | Eva     | HR         |  42000 |
|          6 | Frank   | IT         |  55000 |

Q10:
Write an SQL query to display the Name of employees whose name starts with the letter A.

🔵Query:
SELECT Name
FROM Employees
WHERE Name LIKE 'A%';

⭐Output:

| Name  |
| ----- |
| Alice |

Use this Employees table:
| EmployeeID | Name    | Department | Salary |
| ---------: | ------- | ---------- | -----: |
|          1 | Alice   | HR         |  40000 |
|          2 | Bob     | IT         |  50000 |
|          3 | Charlie | Finance    |  45000 |
|          4 | David   | IT         |  60000 |
|          5 | Eva     | HR         |  42000 |
|          6 | Frank   | IT         |  55000 |


Q11:
Write an SQL query to display the Name and Salary of all employees whose salary is greater than 45,000, and sort the result from highest salary to lowest salary.

🔵Query:
SELECT Name, Salary
FROM Employees
WHERE Salary > 45000
ORDER BY Salary DESC;

⭐Output:
| Name  | Salary |
| ----- | -----: |
| David | 60,000 |
| Frank | 55,000 |
| Bob   | 50,000 |

Use this Employees table:
| EmployeeID | Name    | Department | Salary |
| ---------: | ------- | ---------- | -----: |
|          1 | Alice   | HR         |  40000 |
|          2 | Bob     | IT         |  50000 |
|          3 | Charlie | Finance    |  45000 |
|          4 | David   | IT         |  60000 |
|          5 | Eva     | HR         |  42000 |
|          6 | Frank   | IT         |  55000 |


Q12:
Write an SQL query to display the Department and the number of employees in each department.

🔵Query:
SELECT Department, COUNT(*)
FROM Employees
GROUP BY Department;

⭐Output:
| Department | Employee Count |
| ---------- | -------------: |
| HR         |              2 |
| IT         |              3 |
| Finance    |              1 |



Use this table Employee:
| EmployeeID | Name    | Department | Salary |
| ---------: | ------- | ---------- | -----: |
|          1 | Alice   | HR         |  40000 |
|          2 | Bob     | IT         |  50000 |
|          3 | Charlie | Finance    |  45000 |
|          4 | David   | IT         |  60000 |
|          5 | Eva     | HR         |  42000 |
|          6 | Frank   | IT         |  55000 |


Q13:
Write an SQL query to display each Department and the average salary of employees in that department.

🔵Query:
SELECT Department, AVG(Salary) AS Average_Salary
FROM Employees
GROUP BY Department;

⭐Output:
| Department | Average_Salary |
| ---------- | -------------: |
| HR         |         41,000 |
| IT         |         55,000 |
| Finance    |         45,000 |

Use this Employees table:
| EmployeeID | Name    | Department | Salary |
| ---------: | ------- | ---------- | -----: |
|          1 | Alice   | HR         |  40000 |
|          2 | Bob     | IT         |  50000 |
|          3 | Charlie | Finance    |  45000 |
|          4 | David   | IT         |  60000 |
|          5 | Eva     | HR         |  42000 |
|          6 | Frank   | IT         |  55000 |



🔵Query:

SELECT Department, AVG(Salary) AS AverageSalary
FROM Employees
GROUP BY Department
HAVING AVG(Salary) > 45000;


⭐Output:

| Department | AverageSalary |
| ---------- | ------------: |
| IT         |        55,000 |


Use this table: Employees:

| EmployeeID | Name    | Department | Salary |
| ---------: | ------- | ---------- | -----: |
|          1 | Alice   | HR         |  40000 |
|          2 | Bob     | IT         |  50000 |
|          3 | Charlie | Finance    |  45000 |
|          4 | David   | IT         |  60000 |
|          5 | Eva     | HR         |  42000 |
|          6 | Frank   | IT         |  55000 |

🔵Query:
SELECT Name, Salary 
FROM employees 
WHERE Salary > 45000 
ORDER BY Salary DESC;

⭐Output:

| Name  | Salary |
| ----- | -----: |
| David | 60,000 |
| Frank | 55,000 |
| Bob   | 50,000 |
