# SQL Cheatsheet

### SQL terminal commands
| Command | Description |
| ----------- | ----------- |
| psq| Enter PSQ on terminal|
|\q|Exit|
|cmd K|Clear screen|
|ctrl C| Stop query|
|CREATE DATABASE NewDatabaseName| Create new database|
|DROP DATABASE DatabaseName|Delete a database|
|\c databaseName| change to a different database|
|\l| Shows all current databases|


## Main Data Types
| SQL | Description |
| ----------- | ----------- |
| INT         | Whole Numbers |
|DECIMAL (M, N) |     Decimal Numbers - Exact Value
|VARCHAR(1)     |    String of text with length 1
|BLOB           |   Binary Large Object, Stores large data
|DATE           |   "YYYY-MM-DD"
|TIMESTAMP      |  "YYYY-MM-DD HH:MM:SS"

## Creating a new table in a databse

#### CREATE TABLE table_name (column_name DATATYPE,column_name DATATYPE);

### example:  CREATE TABLE movies (
    id SERIAL,
    title VARCHAR(255),
    duration INT,
    rating VARCHAR(255)
);
