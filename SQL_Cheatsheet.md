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
|DECIMAL (d) |     Decimal Numbers - Exact fixed-point  number
|TEXT| String of max length 65,535 bytes|
|VARCHAR    |    String of text with length 1
|BLOB           |   Binary Large Object, Stores large data
|DATE           |   "YYYY-MM-DD"
|TIMESTAMP      |  "YYYY-MM-DD HH:MM:SS"

##DATATYPE Constraints
| Constraint | Description |
| ----------- | ----------- |
| Not Null (NN)|Ensures that a column cannot have a NULL value|
|UNIQUE|Ensures that all values in a column are different|
|PRIMARY KEY|A combination of a NOT NULL and UNIQUE. Uniquely identifies each row in a table|
|FOREIGN KEY|Prevents actions that would destroy links between tables|
|CHECK|Ensures that the values in a column satisfies a specific condition|
|DEFAULT|Sets a default value for a column if no value is specified|
|CREATE INDEX|Used to create and retrieve data from the database very quickly
|

## Creating a new table in a databse


CREATE TABLE table_name (\
    column1 datatype constraint,\
    column2 datatype constraint,\
    column3 datatype constraint,\
    ....
);


### example: 

### CREATE TABLE movies (
    id SERIAL NN,
    title VARCHAR(255),
    duration INT,
    rating VARCHAR(255)
);

## BASIC OPERATIONS - CRUD
CREATE - READ - UPDATE - DELETE


