# SQL_training

## My SQL training commands


#### CREATE DATABASE
```
CREATE DATABASE my_first_database; # to create a database
```

#### SHOW DATABASES
```
SHOW DATABASES; # to show all the databases available
```

#### USE database
```
USE my_first_database; # to enter the database needed
```

#### CREATE TABLE with columns
```CREATE TABLE person(

  -id INT,

  -first_name VARCHAR(20),

  -last_name VARCHAR(20)

  );
```
  #to create a table called person that has columns: id numeric, first_name in text (20) and last name (20)

#### INT PRIMARY KEY AUTO_INCREMENT
``` id INT PRIMARY KEY AUTO_INCREMENT #to put the numbers into the first column for counting
```

#### SHOW TABLES
```
  SHOW TABLES; #to show all available tables in the current databases
```

#### SELECT everything FROM table
```
SELECT * FROM person; # to select everything from a specified table and demonstrate it (or read it)

SELECT s_first_name, age FROM people; #to read or see only first name and age of people

SELECT * FROM table WHERE name = 'Anastasia'; #to read and see the column with the name Anastasia

SELECT * FROM table WHERE age > 17; #to read data where students are older than 17

SELECT brand FROM table WHERE ram > 8; # to read only those brands where ram is  greater than 8
```
#### DROP TABLE
```
DROP TABLE person; #to delete a complete table called person
```

#### ALTER TABLE table (adding and deleting columns)
```
ALTER TABLE person ADD new_column_name DECIMAL(3,2); # to add a new column to the table person and name the column in fractures (3,2)

ALTER TABLE person DROP COLUMN existing_column_name; #to delete one specified column from the specified table called person
```
#### INSERT INTO table VALUES
```
INSERT INTO my_table VALUES(val1_column1, val2_column2, ... val_columnN); #insert data into the rows for all columns

INSERT INTO my_table  VALUES(id, first_name, last_name) VALUES(3,'Anna','Smith');
#to insert data into some specific columns and not in the ones you have numbers (id)
```

#### UPDATE table SET
```UPDATE table SET my_column = 'newValue';
#to modify the column my_column with new VALUES

UPDATE student SET description = 'he studied well' WHERE s_name = 'John';
#to modify the column description with the wording 'he studied well' for the student John

UPDATE product SET price=100 WHERE name LIKE '%pants%';
#to modify the column price with 100 for all the items with 'pants' - like Nike pants, Adidas pants, etc.

UPDATE computer SET ram=100 WHERE brand IN('Apple','Samsung','Asus');
#to modify column ram with 100 for all the specified brands - Apple, Samsung, Asus
```

#### DELETE FROM
```
DELETE FROM student; #to delete the table student

DELETE FROM student WHERE name='John'; #to delete data only from the column with the name John

DELETE FROM  computer WHERE age=12  AND brand='Asus'; #to delete from columns where age=12 and brand is Asus
```

#### TRUNCATE table

```
TRUNCATE student; #to delete all data from all table called student
```

#### JOIN
```
SELECT m.column_1,f.column_2
FROM members m
INNER JOIN footballers f USING(name)
or
INNER JOIN footballers f ON m.name=f.name;
#create a new table with the column_1 and column_2 using the matching part m.name=f.s_name
```

#### LEFT JOIN
#all the same, but plus include the remaining rows from LEFT table

#### RIGHT JOIN
#all the same, but plus include the remaining rows from the RIGHT table

#### FULL OUTER JOIN
#all the same, but plus include the remaining rows from both left and right tables
