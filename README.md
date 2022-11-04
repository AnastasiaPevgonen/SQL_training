# SQL_training
My SQL training commands

CREATE DATABASE my_first_database; # to create a database

SHOW DATABASES; # to show all the databases available

USE my_first_database; # to enter the database needed

CREATE TABLE person(

  -id INT,

  -first_name VARCHAR(20),

  -last_name VARCHAR(20)

  );

  #to create a table with called person that has columns: id numeric, fist name in text (20) and last name (20)

  SHOW TABLES; #to show all available tables in the current databases

  SELECT * FROM person; # to select everything form a specified table and demonstrate it

DROP TABLE person; #to delete a complete table person

ALTER TABLE person ADD new_column_name DECIMAL(3,2); # to add a new column to the table person and name the column in text (20)

ALTER TABLE person DROP COLUMN existing_column_name; #to delete one specified column from the specified table person

INSERT INTO my_table VALUES(val1_column1, val2_column2, ... val_columnN); #insert data into the rows for each specific column

INSERT INTO my_table  VALUES(id, first_name, last_name) VALUES(3,'Anna','Smith');
#to insert data into some specific columns and not in the ones you have no

SELECT s_first_name, age FROM people; #to read or see only first name and age of people

INT PRIMARY KEY AUTO_INCREMENT #to out the numbers into  the columns

SELECT * FROM table WHERE name = 'Anastasia'; #to read and see the column with the name Anastasia

SELECT * FROM table WHERE age > 17; #to read data where students are older than 17

SELECT brand FROM table WHERE ram = 8; # to read only those brands where ram is  greater than 8

UPDATE table SET my_column = 'newValue';
#to modify the column my_column with a new VALUES

UPDATE student SET description = 'he studied well' WHERE s_name = 'John';
#to modify the column description with the wording 'he studied well' for the student John

UPDATE product SET price=100 WHERE name LIKE '%pants%';
#to modify the column price with 100 for all the items with 'pants' - like Nike pants, Adidas pants, etc.

UPDATE computer SET ram=100 WHERE brand IN('Apple','Samsung','Asus');
#to modify column ram with 100 for all the specified brands - Apple, Samsung, Asus
