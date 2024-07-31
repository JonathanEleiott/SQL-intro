# SQL && Database Basics

## Types of Databases

- Relational
  - Uses tables made up of columns and rows
    - row = record (actual data)
    - column = field
    - Column Types
      - INTEGER - whole numbers
      - FLOAT (totalNumbers, afterDecimal) - numbers with decimals
      - CHAR (numberOfCharacters) - string with the exact character count
      - VARCHAR (numberOfCharacters) - string up to the # of characters
      - DATE - date
      - BOOLEAN - true or false (1 or 0)
      - TEXT - large amounts of text
      - NULLABLE - null
    - Primary Keys - unique identifier for each record (key in React, id)
      - cannot be NULL
      - a table can only have one
    - Foreign Keys
      - link two tables
      - references the primary key of another table
    - Relationships
      - one-to-one
        - state - capitol
        - city - mayor
        - city - address
      - one-to-many or many-to-one
        - archaeological site -< artifacts
        - brand -< products
        - teacher -< students
      - many-to-many
        - teachers >-< students
        - books >-< authors
        - products >-< users
        - doctors >-< patients
    - Join/Junction Table
      - many-tomany relationships

- NoSQL (not only SQL)
  - everything else

- PostgreSQL (database software)
  - relational database

## SQL (Structured Query Language)

- language of the database
- SQL Queries - tell the db what we want to do (MUST END IN SEMICOLON)
  - SELECT - select which table to start retriving records from
    - coumn_1, column_2, ... - which columns to grab
    - FROM - which table to start from
    - table_name - name of the table to start from
    - ex: SELECT name, address FROM residents;
    - ex: SELECT * FROM pets;
    - ex: SELECT name FROM capitols;
    - give us back a new table with the information that we ask for
  - WHERE column = value - filters out the records we don't want
  - JOIN table ON relationship

- Database
  - CREATE DATABASE databasename;
  - DROP - delete the database
- Tables
  - CREATE TABLE table_name ( column1 column_type )
  - ALTER - modify existing table
  - DROP - delete a table
- Rows
  - INSERT INTO table_name (column1, column2) VALUES (value1, value2) - add a new record (row)
  - UPDATE - modify a record
  - DELETE - removes a record
