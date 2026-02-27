# DBMS Project – Oracle 19c
## Music Industry Management System
---
Varianta in Romana: [README.md](README.md)

## General Description
This project implements a relational database designed to manage activities within the music industry, including artists, albums, songs, music genres, sales, managers, and distributors.

The solution includes conceptual and logical database modeling, implementation in Oracle Database 19c, and development of advanced PL/SQL components.

## Database Modeling
The project includes:
- Conceptual diagram
- Entity–Relationship diagram
- SQL scripts for:
  - Table creation
  - Constraints definition (primary keys, foreign keys, integrity constraints)
  - Test data insertion

## Implemented Features

### Procedures and Functions
- Monthly artist report procedure (using VARRAY, Nested Table, and Associative Array collections)
- Cursor-based reporting procedure (implicit and parameterized cursors)
- Function for calculating sale value with predefined exception handling:
  - NO_DATA_FOUND
  - TOO_MANY_ROWS
  - OTHERS
- Complex procedure with user-defined exceptions

### PL/SQL Collections Used
- VARRAY
- Nested Table
- Associative Array (INDEX BY)

### Cursors
- Implicit cursor (FOR SELECT statement)
- Explicit parameterized cursor

### Triggers
- DML trigger preventing DELETE operations during weekends
- Compound trigger counting affected rows and calculating total deleted value
- DDL trigger preventing DROP TABLE operations at schema level

## Technologies Used
- Oracle Database 19c
- PL/SQL
- SQL Developer

## Project Structure
/sql – SQL and PL/SQL scripts  
/diagrams – database diagrams  
/doc – project documentation  

## Purpose
Developed as part of a Database Management Systems course.

## Author
Ardeleanu-Chirica Matei
