# Learning-SQL
<strong>This repository contains my notes, exercises, and projects as I learn SQL. It's designed to help who are new to SQL get started with this powerful language. I'll be sharing short and easy-to-understand explanations of key concepts, as well as code examples and queries that demonstrate how to use SQL to solve real-world problems. Join me on my journey to become an SQL pro!</strong>
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/c5e6b0447c2456eb0f48901c5370d9b730ae5780/image/sql.jpg)
# Day1
### What is SQl ?
SQL is a standard language for storing, manipulating and retrieving data in databases.
* **Database:** Database is a repository of data that contains collection of data in a structured ways.
* **Relational database:** Data stored in forms of rows and columns is called relational database .
* **RDBMS:** A relational database management system (RDBMS) is a program used to create, update, and manage relational databases.

## SELECT
Select statement is used to retrieve data from database .
Let see a syntax:
```SQL
SELECT column1, column2, ...
FROM table_name
WHERE condition
;
```
* SELECT:Is used to select data specified by attributes
* WHERE: Filters data according to condition
* FROM: From is used to specify location of data
Here is sample program :
![Sample program](https://github.com/Utshav-paudel/Learning-SQL/blob/396c5955c91c1a28587883705087a4bd39d4be46/image/day1.png)
# Day2
:large_blue_diamond: COUNT:
COUNT() is a built in function that retrieves the number of rows that matches the query crietaria .
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/860902eb2c60d0c6a81713bf0e893fe89b2e5cb0/image/day%202%20COUNT.png)

:large_blue_diamond: DISTINCT:
The ```SELECT DISTINCT``` statement is used to return only distinct (different) values.
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/860902eb2c60d0c6a81713bf0e893fe89b2e5cb0/image/day2%20DISTINCT.png)

:large_blue_diamond:LIMIT: 
LIMIT is used for restricting the number of rows retrieved from databases.
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/860902eb2c60d0c6a81713bf0e893fe89b2e5cb0/image/day2%20LIMIT.png)

# Day3
## INSERT
This statement is used to add new rows to a table
syntax:
```SQL
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);
```

## UPDATE
This statement is used to modify the existing records in a table.
Syntax:
```SQL
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```
**Warning** : If you use update statement without WHERE clause it will change all records in the table

![https://github.com/Utshav-paudel/Learning-SQL/blob/dcd3cc237d9fe038885648c966c43063adffc712/image/day3%20meme.jpg](https://github.com/Utshav-paudel/Learning-SQL/blob/dcd3cc237d9fe038885648c966c43063adffc712/image/day3%20meme.jpg)

## DELETE
This statement is used to delete the existing records from a table .
Syntax:
```SQL
DELETE FROM table_name WHERE condition;
```

# Day4
Today I have revised all concepts of SQL from previous days and here is a cheatsheet of statement used in sql:

![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/1b8dbbac687bff11d4209511b168c63d7e133966/image/day4%20cheatsheet.png)

After revision I learn about :
* **Relational database model**<br>
It is database where data is stored in tables.
* **Entity Relationship model**<br>
Entity are tables and attributes are columns.<br>
For e.g: If book is entity then its title,price,page,author all this are attributes
* **Primary keys and foreign keys**<br>
Primary keys are unique key that identifes the rows in a table.<br>
Foreign keys are primary key from another table that helps to create relationship.
## Types of SQL statement
### 1.DDL statement(Data Definition Language)
Used for definition of table,change or drop data .
* CREATE
* ALTER
* TRUNCATE
* DROP<br>
### 2.DML statement(Data Manipulation Language)
Used for read and modifying of data i.e manipulation of data .
* INSERT
* SELECT
* UPDATE
* DELETE<br>
we had already learned about DML statement .
Today we will start with DDL statement.

### CREATE
It is used to create table in a database.
syntax:
```SQL
CREATE TABLE table_name (
    column1 datatype,
    column2 datatype,
    column3 datatype,
   ....
);
```
# Day5
Today I continued DDL statement ,
### ALTER 
It is used to add or remove columns,keys,constraints and modify the data types of columns.<br>
Syntax:
```SQL  
ALTER TABLE table_name
ADD column_name datatype;
```
### DROP 
It is used to drop existing table from the databases.
<br>
Syntax:
```SQL
DROP TABLE table_name;
```
### TRUNCATE
It is used to delete the data inside the table but not the table itself.
<br>
Syntax:
```SQL
TRUNCATE TABLE table_name;
```

### Cheatsheet for DDL statement
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/06a923b57ca5b2ecf59b3e01596a7b1f23d56dbf/image/day5%20cheatsheet%20of%20ddl.png)

# Day6
### String Patterns,Ranges and sets

When we exactly don't know what predicate to use with WHERE clause we use String patterns,Ranges and sets.
LIKE and NOT LIKE are some example of string patterns
Before learning about them lets see some symbol and their representation:
<br>
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/61742a652e0a4243ee7145b4f9f714d3dfff8bc6/image/day6%20character%20and%20it%20meaning.png)
<br>
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/61742a652e0a4243ee7145b4f9f714d3dfff8bc6/image/day6%20example%20pattern%20and%20meaning.png)
### String patterns
* LIKE
```SQL
SELECT name FROM planets
  WHERE name LIKE "%us";
  ```
* NOT LIKE
```SQL
SELECT name FROM planets
  WHERE name NOT LIKE "%u%";
```

### Range
Range is used with where clause as follow:
```SQL
SELECT * FROM employees WHERE salary BETWEEN 40000 AND 80000;
```
# Day7
Today I learning about various method that helps to retrieve data from database or sort data according to user requirement
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/1b75e61d2d866f3cb70e389e9eb5a567a9d80a12/image/day7%20sorting%20.png)

# Day8

Today I learned about built in function in SQL.
### Aggregate or column functions.
This functions take columns as input and return single value output.
* SUM(),MIN(),MAX(),AVG().<br>
Syntax:<br>
```SQL
SELECT SUM(COLUMN_NAME) FROM TABLE_NAME;
```
### Scalar and string function.
This functions perform operation on every input value.<br>
* ROUND(),LENGTH(),UCASE,LCASE<br>
Syntax:

```SQL
SELECT f_name FROM employee
WHERE LCASE(ADDRESS)="kathmandu";
```

### Date and time built in functions
* YEAR(),MONTH(),DAY(),DAYOFMONTH(),DAYOFYEAR(),DAYOFWEEK(),WEEK(),HOUR(),MINUTE(),SECOND()


# Day9
Today I learned about the subqueries in SQL.<br>
### **subquery**:
A subquery is a SQL query nested inside a larger query.
A subquery may occur in :
* A SELECT clause
* A FROM clause
* A WHERE clause
Syntax:

![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/db82ebc7821b890fbc4e6afb7cc6ca50e692bc47/image/day9%20subquery%20syntax.png)

# Day10

Today, I learned about how to work with multiple tables in SQL. Here are some of the key points I learned:

* In a relational database, information is often stored in multiple tables to avoid redundancy and ensure data consistency.
* This means that we need to use SQL queries that combine data from multiple tables in order to answer certain questions.
* To do this, we can use SQL JOIN statements, which allow us to combine rows from two or more tables based on a related column between them.
* There are several types of JOINs, including INNER JOIN, LEFT JOIN, RIGHT JOIN, and FULL OUTER JOIN. Each type of JOIN behaves slightly differently and can be used in different scenarios.
*When working with multiple tables, it's important to understand how the tables are related to each other. This typically involves looking at the foreign key columns that link the tables together.
*By using JOINs and other SQL techniques like using subqueries and implicit join , we can extract valuable insights and answers from even the most complex data sets. Working with multiple tables in SQL can be complex, but it's an essential skill for anyone working with relational databases.

# Cheatsheet for built in function and working with multiple table
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/f4eba55e485ef827f04aa267df4d3263d3b90d58/image/day10%20cheatsheet.png)
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/f4eba55e485ef827f04aa267df4d3263d3b90d58/image/day10.1%20cheatsheet.png)

# Day11
Today, I learned about db-api that let us allow to use database using python .

# DB API module
This module provides a simple and consistent interface to connect to a database and execute SQL statements using the Python DB API 2.0 specification.
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/d43a8bffc299e75510061302ae4badb035904224/image/day11%20dbapi.jpg)

[Here](https://github.com/Utshav-paudel/Learning-SQL/blob/d43a8bffc299e75510061302ae4badb035904224/code/Creating%20tables,inserting%20data%20and%20querying.ipynb) is sample of creating table,inserting query in DB Api from jupyter notebook.

# Day12
Today I learned about SQL magic
* SQL Magic is a feature in Jupyter Notebook and JupyterLab that allows users to execute SQL commands directly within the notebook environment. It is a Jupyter extension that enables users to interact with databases using SQL commands, and to display the results of those commands in the notebook.

* With SQL Magic, users can connect to a variety of databases, such as MySQL, PostgreSQL, SQLite, and Oracle, and execute SQL queries to retrieve, filter, and aggregate data. The results of the queries can be displayed in various formats, such as tables, charts, or graphs, using visualization libraries like Matplotlib or Seaborn.

* SQL Magic simplifies the process of data analysis and manipulation by providing an easy-to-use interface for executing SQL commands in a notebook environment. It allows users to seamlessly integrate SQL with other programming languages like Python, R, or Julia, and to share their SQL code and results with others using Jupyter notebooks.
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/02161cc1d45fee7c6c9d1019d531adbefc6adcc1/image/day12%20sql%20magic.jpeg)

[here](https://github.com/Utshav-paudel/Learning-SQL/blob/bf91994024373293bd344a46e09907e58fb4ad92/code/Accessing%20database%20using%20sql%20magic.ipynb) is sample of accessing database using SQL magic

# Day13
Today I learned about using sql in jupyternotebook. 
* <strong>QUERYING  column names with mixed (upper and lower) case.</strong>

use double quote for e.g
```select "Id" from dog```
* <strong>QUERYING column names with spaces and special characters.</strong>
Use underscores to map spaces and other characters. for e.g:
```Breed (dominant)``` is written as ```Breed__dominant_```
* <strong>Splitting queries in multiple line in jupyter</strong>
1. In case of %sql , use backslash.
2. In case of %%sql , no need of backslash.
* <strong>Restricitng numbers of rows retrieving from databases.</strong>  
Use LIMIT function.
* <strong>Getting a list of tables in the databases</strong>
1. Db2  
Use SYSCAT.TABLES
2. SQL serverd  
use INFORMATION_SCHEMA.TABLES
3. Oracle  
ALL_TABLES or USER_TABLES
