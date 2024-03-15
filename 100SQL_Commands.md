### 100 SQL Commands
1. ###### SELECT 
   - retrieves data from a database

1. ###### INSERT 
   - inserts new data into a database

1. ###### UPDATE 
   - updates existing data in a database

1. ###### DELETE 
   - deletes data from a database

1. ###### CREATE DATABASE 
   - creates a new database

1. ###### CREATE TABLE 
   - creates a new table in a database

1. ###### ALTER TABLE 
   - modifies an existing table structure

1. ###### DROP TABLE 
   - deletes a table from a database

1. ###### TRUNCATE TABLE 
   - removes all records from a table

1. ###### CREATE INDEX 
   - creates an index on a table

1. ###### DROP INDEX 
   - deletes an index from a table

1. ###### JOIN 
   - combines rows from two or more tables based on a related column

1. ###### INNER JOIN 
   - returns rows when there is a match in both tables

1. ###### LEFT JOIN 
   - returns all rows from the left table, and the matched rows from the right table

1. ###### RIGHT JOIN 
   - returns all rows from the right table, and the matched rows from the left table

1. ###### FULL JOIN 
   - returns rows when there is a match in one of the tables

1. ###### UNION 
   - combines the results of two or more SELECT statements

1. ###### UNION ALL 
   - combines the results of two or more SELECT statements, including duplicates

1. ###### GROUP BY 
   - groups rows that have the same values into summary rows @code._learning

1. ###### HAVING 
   - filters records based on a specified condition

1. ###### ORDER BY 
   - sorts the result set in ascending or descending order

1. ###### COUNT 
   - returns the number of rows that satisfy the condition

1. ###### SUM
   - calculates the sum of a set of values

1. ###### AVG 
   - calculates the average of a set of values

1. ###### MIN 
   - returns the smallest value in a set of values

1. ###### MAX 
   - returns the largest value in a set of values

1. ###### DISTINCT 
   - selects unique values from a column

1. ###### WHERE 
   - filters records based on specified conditions

1. ###### AND 
   - combines multiple conditions in a WHERE clause

1. ###### OR 
   - specifies multiple alternative conditions in a WHERE clause

1. ###### NOT 
   - negates a condition in a WHERE clause

1. ###### BETWEEN 
   - selects values within a specified range

1. ###### IN 
   - specifies multiple values for a column

1. ###### LIKE 
   - selects rows that match a specified pattern

1. ###### IS NULL 
   - checks for NULL values in a column

1. ###### IS NOT NULL 
   - checks for non-NULL values in a column

1. ###### EXISTS 
   - tests for the existence of any record in a subquery

1. ###### CASE 
   - performs conditional logic in SQL statements

1. ###### WHEN 
   - specifies conditions in a CASE statement

1. ###### THEN 
   - specifies the result if a condition is true in a CASE statement

1. ###### ELSE 
   - specifies the result if no condition is true in a CASE statement

1. ###### END 
   - ends the CASE statement

1. ###### PRIMARY KEY 
   - uniquely identifies each record in a table

1. ###### FOREIGN KEY 
   - establishes a relationship between tables

1. ###### CONSTRAINT 
   - enforces rules for data in a table

1. ###### DEFAULT 
   - specifies a default value for a column

1. ###### NOT NULL 
   - ensures that a column cannot contain NULL values

1. ###### UNIQUE 
   - ensures that all values in a column are unique

1. ###### CHECK 
   - enforces a condition on the values in a column

1. ###### CASCADE 
   - automatically performs a specified action on related records

1. ###### SET NULL 
   - sets the value of foreign key columns to NULL when a referenced record is deleted 

1. ###### SET DEFAULT 
   - sets the value of foreign key columns to their default value when a referenced record is deleted

1. ###### NO ACTION 
   - specifies that no action should be taken on related records when a referenced record is deleted

1. ###### RESTRICT 
   - restricts the deletion of a referenced record if there are related records

1. ###### CASE WHEN 
   - conditional expression in SELECT statements

1. ###### WITH 
   - defines a common table expression (CTE)

1. ###### INTO 
   - specifies a target table for the result set of a SELECT statement

1. ###### TOP 
   - limits the number of rows returned by a query

1. ###### LIMIT 
   - limits the number of rows returned by a query (used in some SQL dialects)

1. ###### OFFSET 
   - specifies the number of rows to skip before starting to return rows

1. ###### FETCH 
   - retrieves rows from a result set one at a time

1. ###### ROW_NUMBER() 
   - assigns a unique sequential integer to each row in a result set

1. ###### RANK() 
   - assigns a unique rank to each row in a result set, with gaps in the ranking sequence possible

1. ###### DENSE_RANK() 
   - assigns a unique rank to each row in a result set, with no gaps in the ranking sequence

1. ###### NTILE() 
   - divides the result set into a specified number of equally sized groups

1. ###### LEAD() 
   - retrieves the value from the next row in a result set

1. ###### LAG() 
   - retrieves the value from the previous row in a result set

1. ###### PARTITION BY 
   - divides the result set into partitions to which the window function is applied separately

1. ###### ORDER BY 
   - specifies the order of rows within each partition for window functions

1. ###### ROWS 
   - specifies the window frame for window functions

1. ###### RANGE 
   - specifies the window frame based on values rather than rows for window functions

1. ###### CURRENT TIMESTAMP 
   - returns the current date and time

1. ###### CURRENT_DATE 
   - returns the current date

1. ###### CURRENT_TIME 
   - returns the current time

1. ###### DATEADD 
   - adds a specified time interval to a date

1. ###### DATEDIFF 
   - calculates the difference between two dates

1. ###### DATEPART 
   - extracts a specific part of a date

1. ###### GETDATE 
   - returns the current date and time (similar to CURRENT_TIMESTAMP)

1. ###### GROUPING SETS 
   - specifies multiple groupings for aggregation

1. ###### CUBE 
   - generates all possible combinations of grouping sets for aggregation

1. ###### ROLLUP 
   - generates subtotal values for a hierarchy of values

1. ###### INTERSECT 
   - returns the intersection of two result sets

1. ###### EXCEPT 
   - returns the difference between two result sets

1. ###### MERGE 
   - performs insert, update, or delete operations on a target table based on the results of a join with a source table

1. ###### CROSS APPLY 
   - performs a correlated subquery against each row of the outer table

1. ###### OUTER APPLY 
   - similar to CROSS APPLY, but also returns rows from the outer table that have no matching rows in the inner table

1. ###### PIVOT 
   - rotates a table-valued expression by turning the unique values from one column into multiple columns in the output

1. ###### UNPIVOT 
   - rotates a table-valued expression by turning multiple columns into unique rows in the output

1. ###### COALESCE 
   - returns the first non-NULL expression in a list

1. ###### NULLIF 
   - returns NULL if the two specified expressions are equal, otherwise returns the first expression

1. ###### IIF 
   - returns one of two values based on a Boolean expression 

1. ###### CONCAT 
   - concatenates two or more strings

1. ###### SUBSTRING 
   - extracts a substring from a string

1. ###### CHARINDEX 
   - finds the position of a substring within a string

1. ###### REPLACE 
   - replaces all occurrences of a specified substring within a string with another substring

1. ###### LEN 
   - returns the length of a string

1. ###### UPPER 
   - converts a string to uppercase

1. ###### LOWER 
   - converts a string to lowercase

1. ###### TRIM 
   - removes leading and trailing spaces from a string

1. ###### ROUND 
   - rounds a numeric value to a specified number of decimal places