## Table of Content

| No  | Content                               | No  | Content                                     | No  | Content                                     |
| --- | ------------------------------------- | --- | ------------------------------------------- | --- | ------------------------------------------- |
| 1.  | [Create Database](#1create-database)  | 2.  | [Create Table](#2create-table)              | 3.  | [NOT NULL](#3sql-constraint-not-null)       |
| 4.  | [UNIQUE](#4sql-constraint-unique)     | 5.  | [PRIMARY KEY](#5sql-constraint-primary-key) | 6.  | [FOREIGN KEY](#6sql-constraint-foreign-key) |
| 7.  | [CHECK](#7sql-constraint-check)       | 8.  | [DEFAULT](#8sql-constraint-default)         | 9.  | [ALTER TABLE](#9alter-table-command)        |
| 10. | [INSERT INTO](#10insert-into-command) | 11. | [SELECT Command](#11select-command)         |

#### 1.Create Database

```sql

CREATE DATABASE `database name`;

CREATE DATABASE db1;
```

##

#### 2.Create Table

```sql

CREATE TABLE `table name`(
    columns
);

CREATE TABLE employee(
    id INT,
    name VARCHAR(255)
);
```

##

#### 3.SQL Constraint NOT NULL

##

#### 4.SQL Constraint UNIQUE

##

#### 5.SQL Constraint PRIMARY KEY

- Quick Reference

```sql
CREATE TABLE employee(
    empid INT PRIMARY KEY AUTO_INCREMENT,
    depart_id INT,
    name VARCHAR(255),
    FOREIGN KEY (depart_id) REFERENCES depart_tb(depart_id)
);

After Created Table using Alter;
ALTER TABLE employee add constraint pk_employee PRIMARY KEY(empid);

Delete/Remove Foreign Key;
ALTER TABLE employee DROP PRIMARY KEY;
```

- With Example

```sql
show databases;
use db1;
show tables;

+---------------+
| Tables_in_db1 |
+---------------+
| employee      |
+---------------+

describe employee;

+--------+--------------+------+-----+---------+-------+
| Field  | Type         | Null | Key | Default | Extra |
+--------+--------------+------+-----+---------+-------+
| empid  | int          | YES  |     | NULL    |       |
| name   | varchar(255) | YES  |     | NULL    |       |
| age    | int          | YES  |     | NULL    |       |
| salary | float        | YES  |     | NULL    |       |
+--------+--------------+------+-----+---------+-------+

alter table employee add constraint pk_employee prima
ry key(empid);

Error: Invalid use of NULL value
delete from employee where empid is null;

alter table employee add constraint pk_employee prima
ry key(empid);
describe employee;

+--------+--------------+------+-----+---------+-------+
| Field  | Type         | Null | Key | Default | Extra |
+--------+--------------+------+-----+---------+-------+
| empid  | int          | NO   | PRI | NULL    |       |
| name   | varchar(255) | YES  |     | NULL    |       |
| age    | int          | YES  |     | NULL    |       |
| salary | float        | YES  |     | NULL    |       |
+--------+--------------+------+-----+---------+-------+

alter table employee
    -> drop primary key;

+--------+--------------+------+-----+---------+-------+
| Field  | Type         | Null | Key | Default | Extra |
+--------+--------------+------+-----+---------+-------+
| empid  | int          | NO   |     | NULL    |       |
| name   | varchar(255) | YES  |     | NULL    |       |
| age    | int          | YES  |     | NULL    |       |
| salary | float        | YES  |     | NULL    |       |
+--------+--------------+------+-----+---------+-------+
```

##

#### 6.SQL Constraint FOREIGN KEY

##

#### 7.SQL Constraint CHECK

##

#### 8.SQL Constraint DEFAULT

##

#### 9.ALTER TABLE Command

##

#### 10.INSERT INTO Command

##

#### 11.SELECT Command
