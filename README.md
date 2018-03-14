# **DatabaseSystems**
Database Systems practices with T-SQL using Microsoft SQL Server

# Introduction to Databases

## What Is Database?
Collection of information (data).

## Database Structures
1. **Hierarchical**

It consists of parent-child relationships. Parent nodes can have multiple child nodes. Child nodes, however, can have only one parent node. Therefore, this structure is inflexible.

2. **Network**

It solves the problem of the hierarchical structure. Information is organized by "record types". A record type can work with other record types. It supports complicated searches and relationships. The complexity, however, is the main disadventage; because you need to know how the structure works and how information is stored.

3. **Relational**

The most popular structure. It is a tabular database in which data is defined so that it can be reorganized and accessed in multiple ways. Relational database is made up of a set of tables with data fits into a predefined category.

## Relational Database Management System

The main element of a relational database is the **relation**, which are essentially groups of rows and columns placed in a table that represents one object. 

### Table

Database object that consists of row and colums, and store data. It is the simplest form of data storage in relational databases. Example: CUSTOMERS table

+----+----------+-----+-----------+----------+
| ID | NAME     | AGE | ADDRESS   | SALARY   |
+----+----------+-----+-----------+----------+
|  1 | Ramesh   |  32 | Ahmedabad |  2000.00 |
|  2 | Khilan   |  25 | Delhi     |  1500.00 |
|  3 | kaushik  |  23 | Kota      |  2000.00 |
|  4 | Chaitali |  25 | Mumbai    |  6500.00 |
|  5 | Hardik   |  27 | Bhopal    |  8500.00 |
|  6 | Komal    |  22 | MP        |  4500.00 |
|  7 | Muffy    |  24 | Indore    | 10000.00 |
+----+----------+-----+-----------+----------+

### Field

Smaller entity of a table that is designed to maintain specific information about every recordin the table. Example: ID, NAME, AGE, ADDRESS, SALARY

### Record

A row in a table. Example:

+----+----------+-----+-----------+----------+
|  1 | Ramesh   |  32 | Ahmedabad |  2000.00 |
+----+----------+-----+-----------+----------+

### Column

Vertical entity in a table. Example:

+-----------+
| ADDRESS   |
+-----------+
| Ahmedabad |
| Delhi     |
| Kota      |
| Mumbai    |
| Bhopal    |
| MP        |
| Indore    |
+----+------+

### Data Types (Transact-SQL)

Data types define what type of data a column can contain.

- Exact Numerics
	- bigint, bit, decimal, int, money, numeric, smallint, smallmoney, tinyiny
- Approximate Numerics
	- float, real
- Date and Time
	- date, datetime2, datetime, datetimeoffset, smalldatetime, time
- Character Strings
	- char, text, varchar
- Unicode Character Strings
	- nchar, ntext, nvarchar
- Binary Strings
	- binary, image, varbinary
- Other Data Types
	- cursor, hierarchyid, sql_variant, table, timestamp, uniqueidentifier, xml


### NULL Value

A NULL value is a value in a field that appears to be blank, which means a field with a NULL value is a field with no value. NULL value is different than a zero value or an empty text value. It can be determined and assigned a value in the future.

### SQL Constraints


