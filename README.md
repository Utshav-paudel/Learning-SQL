# Learning-SQL
In this repo I will be uploading my learning on SQL .
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
# Day4
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
```![Uploading day5 cheatsheet of ddl.png…]()

### Cheatsheet for DDL statement
![alt text](https://github.com/Utshav-paudel/Learning-SQL/blob/06a923b57ca5b2ecf59b3e01596a7b1f23d56dbf/image/day5%20cheatsheet%20of%20ddl.png)
