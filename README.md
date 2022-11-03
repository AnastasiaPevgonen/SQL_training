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

ALTER TABLE person ADD new_column-name DECIMAL(3,2); # to add a new column to the table person and name the column in text (20)
