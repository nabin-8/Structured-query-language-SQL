1. What is DATABASE?

- Database is a collection of
data stored in a format that
can easily be accessed.

1. OPERATIONS

- INSERT
- SELECT
- UPDATE
- DELETE

1. SQL
- (Structured Query Language)
SQL is a standard language
for database creation and
manipulation.

1. (Database Management System)

- DBMSis a software or tool that we use to manage our data.

##### Type of DBMS
- Sql
- NoSQl (Relational)

##### RDBMS
- Relational Database Management System

##### Data TYPES
- A database data type refers to the format of data storage that can hold a distinct type 

##### MySQL Data TYPES
|![datatypes](/src/datatypes.png)|
|---|

##### Mysql Workbench installation
##### XAAMP

#### Login Through shell
```
mysql -h localhost -u root
```

#### Create and Drop Database
- sql is not case sensitive langauge
```
CREATE DATABASE mydb;
```
- Use to create database
```
DROP DATABASE mydb;
```
- Use to remove/Delete database

---
#### Tables (Create , Alter, Drop)
- Tables are collection of rows and columns
- To use database
```
use mydb;
```
- Create table in database
```
CREATE TABLE students(
   name varchar(225),
   father_name varchar(225),
   city varchar(50),
   date_of_birth date 
);
```

- Rename table
```
 RENAME TABLE students TO class_students;
```

- Delete table
```
DROP TABLE students;
```

- Alter Table it is used
1. To add new column
1. modify existing column
1. delete any colume

- add new column
```
ALTER TABLE students add class_name varchar(255);
```

- delete column
```
ALTER TABLE students DROP COLUMN  class_name;
```

- MODIFY  column
```
ALTER TABLE students MODIFY COLUMN city varchar(255);
```
- change position of column
```
ALTER TABLE students MODIFY COLUMN date_of_birth date AFTER father_name;
```

- adding colume after any column
```
ALTER TABLE students ADD COLUMN mother_name varchar(255)
AFTER father_name;
```

#### Insert Query
- create new table after drop previous student table
```
 CREATE TABLE students(
     student_id int,
     student_name varchar(255),
     father_name varchar(255),
     marks float(10,2),
     date_of_birth date
     );
```
- Inserting data
```
INSERT INTO students (student_id, student_name, father_name, marks, date_of_birth) VALUES (1,"Nabin", "Shankar", 78.36, "1997-09-10");

INSERT INTO students (student_id, student_name, father_name, marks, date_of_birth) VALUES (2, "Hemant", "hemnath", 89.33, "1988-09-10");
```

- Nth-Number of Query / Multiple Query
```
 INSERT INTO students (student_id, student_name, father_name) VALUES(3, "Joy","smith"),
     (4, "John", "Don")
     ;
```

#### SELECT QUERY
- select query is help to fetch data from database and show to user.

- Show all tables
```
 SELECT * FROM students;

+------------+--------------+-------------+-------+---------------+
| student_id | student_name | father_name | marks | date_of_birth |
+------------+--------------+-------------+-------+---------------+
|          1 | Nabin        | Shankar     | 78.36 | 1997-09-10    |
|          2 | Hemant       | hemnath     | 89.33 | 1988-09-10    |
|          3 | Joy          | smith       |  NULL | NULL          |
|          4 | John         | Don         |  NULL | NULL          |
+------------+--------------+-------------+-------+---------------+
```

- Another Way with specific student_name and father_name.
```
SELECT student_name, father_name FROM students;

+--------------+-------------+
| student_name | father_name |
+--------------+-------------+
| Nabin        | Shankar     |
| Hemant       | hemnath     |
| Joy          | smith       |
| John         | Don         |
+--------------+-------------+
```

#### WHERE CLAUSE
- if i need student data which id have 4 lets see whats the query
```
SELECT * FROM students WHERE student_id=4;

+------------+--------------+-------------+-------+---------------+
| student_id | student_name | father_name | marks | date_of_birth |
+------------+--------------+-------------+-------+---------------+
|          4 | John         | Don         |  NULL | NULL          |
+------------+--------------+-------------+-------+---------------+
```
- number of students marks having Greater than 50

```
SELECT * FROM students WHERE marks >=50;

+------------+--------------+-------------+-------+---------------+
| student_id | student_name | father_name | marks | date_of_birth |
+------------+--------------+-------------+-------+---------------+
|          1 | Nabin        | Shankar     | 78.36 | 1997-09-10    |
|          2 | Hemant       | hemnath     | 89.33 | 1988-09-10    |
+------------+--------------+-------------+-------+---------------+
```

- Find Date of Birth
``` 
 SELECT * FROM STUDENTS WHERE date_of_birth = "1997-09-10";

+------------+--------------+-------------+-------+---------------+
| student_id | student_name | father_name | marks | date_of_birth |
+------------+--------------+-------------+-------+---------------+
|          1 | Nabin        | Shankar     | 78.36 | 1997-09-10    |
+------------+--------------+-------------+-------+---------------+
```

- Students marks greater than 70
```
SELECT student_name FROM students WHERE marks >70;

+--------------+
| student_name |
+--------------+
| Nabin        |
| Hemant       |
+--------------+
```

#### AND, OR, NOT, OPERATORS
