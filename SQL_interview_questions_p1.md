## SQL Interview Question

1. What is SQL?
SQL is a standard database language used for accessing and manipulating data in databases. It stands for Structured Query Language and was developed by IBM Computer Scientists in the 1970s. By executing queries, SQL can create, update, delete, and retrieve data in databases like MySQL, Oracle, PostgreSQL, etc. Overall, SQL is a query language that communicates with databases.

2. What is a database?
A Database is defined as a structured form of data storage in a computer or a collection of data in an organized manner and can be accessed in various ways. The Database Management System allows a user to interact with the database.

3. Does SQL support programming language features?
It is true that SQL is a language, but it does not support programming as it is not a programming language, it is a command language.

4. What is the difference between CHAR and VARCHAR2 datatype in SQL?
Both of these data types are used for characters, but varchar2 is used for character strings of variable length, whereas char is used for character strings of fixed length. For example, if we specify the type as char(5) then we will not be allowed to store a string of any other length in this variable, but if we specify the type of this variable as varchar2(5) then we will be allowed to store strings of variable length. We can store a string of length 3 or 4 or 2 in this variable.

5. What do you mean by data definition language?
Data definition language or DDL allows to execution of queries like CREATE, DROP, and ALTER. That is those queries that define the data.

6. What do you mean by data manipulation language?
Data manipulation Language or DML is used to access or manipulate data in the database. 
It allows us to perform the below-listed functions:
* Insert data or rows in a database
* Delete data from the database
* Retrieve or fetch data
* Update data in a database.

7. What is the view in SQL?  
Views in SQL are a kind of virtual table. A view also has rows and columns as they are on a real table in the database. We can create a view by selecting fields from one or more tables present in the database. A View can either have all the rows of a table or specific rows based on certain conditions.
  CREATE VIEW view_name AS
  SELECT column1, column2.....
  FROM table_name
  WHERE condition;

8. What do you mean by foreign key? 
A Foreign key is a field that can uniquely identify each row in another table. And this constraint is used to specify a field as a Foreign key. That is this field points to the primary key of another table. This usually creates a kind of link between the two tables.
  CREATE TABLE Orders
  (
  O_ID int NOT NULL,
  ORDER_NO int NOT NULL,
  C_ID int,
  PRIMARY KEY (O_ID),
  FOREIGN KEY (C_ID) REFERENCES Customers(C_ID)
  )

9. What is the primary key?
A Primary Key is one of the candidate keys. One of the candidate keys is selected as the most important and becomes the primary key. There cannot be more than one primary key in a table. 

10. What are table and Field?
* Table: A table has a combination of rows and columns. Rows are called records and columns are called fields. In MS SQL Server, the tables are being designated within the database and schema names.
* Field: In DBMS, a database field can be defined as – a single piece of information from a record.
