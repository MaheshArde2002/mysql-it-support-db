# MySQL Database and Table Setup

## Objective

Create a database, create a table, insert sample data, and retrieve the data using SQL commands.

## 1. Login to MySQL

```bash
mysql -u root -p

Enter the MySQL password when prompted.

After successful login:

mysql>
2. Display Existing Databases
SHOW DATABASES;

This command displays the databases available on the MySQL server.

3. Create Database

Create the IT_Support database:

CREATE DATABASE IT_Support;

Verify the database:

SHOW DATABASES;
4. Select Database
USE IT_Support;

Expected output:

Database changed
Note

The following command produced an error because the database name was entered incorrectly:

USE IT_support;

Error:

ERROR 1049 (42000): Unknown database 'IT_support'

The correct database name is:

IT_Support
5. Check Tables
SHOW TABLES;

Initially, the database contains no tables.

6. Create Users Table
CREATE TABLE Users (
    id INT,
    name VARCHAR(20),
    Email VARCHAR(20),
    Department VARCHAR(20)
);
7. Check Table Structure
DESC Users;

The table contains the following columns:

Column	Data Type
id	INT
name	VARCHAR(20)
Email	VARCHAR(20)
Department	VARCHAR(20)
8. Insert Data

Insert a sample record:

INSERT INTO Users
VALUES (1, 'Manoj', 'manoj@gmail.com', 'IT');

Expected output:

Query OK, 1 row affected
SQL Learning Point

The following command produced an error:

INSERT INTO Users VALUES (1, 'Manoj', 'manoj@gmail.com', IT);

Error:

ERROR 1054 (42S22): Unknown column 'IT' in 'field list'

The reason is that IT is a text value and must be enclosed in quotes.

Correct:

'IT'
9. Display Data
SELECT * FROM Users;

Example output:

+------+-------+-----------------+------------+
| id   | name  | Email           | Department |
+------+-------+-----------------+------------+
|    1 | Manoj | manoj@gmail.com | IT         |
+------+-------+-----------------+------------+
Result

The following tasks were completed:

Created IT_Support database
Selected the database
Created Users table
Checked table structure
Inserted sample data
Retrieved data using SELECT

