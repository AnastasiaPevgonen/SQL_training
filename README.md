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
