# What is a Database ? 
- It is a systematic collection of data.

# What is a Primary Key ? 
- It is a unique column in every table in a database.
- Primary key column can only accept non-duplicated values and can't be null.

# What is a Foreign Key ? 
- is key used to link two tables together. Like for ex. We have program_id which will be common for librarian table and student table , so program_id will be the primary key in **programs** table and foreign key in students table. 
- Foreign key is the primary key of another table.

# RDBMS ?
- RDBMS --> Relational Database management system.
- All RDBMS using SQL language. 



# Relational Database ? 
- tables are related to each other using Primary and foreign keys.

# What is the difference between UNION and UNION ALL ?
- PRE-CONDITION FOR UNION AND UNION ALL : SAME COLUMN NAME, COLUMN COUNT, COLUMN DATA TYPE.
  
- Both of them combine the result of 2 queries. And just return combined result
- UNION REMOVES ALL THE DUPLICATES SORTING BY THE 1ST COLUMN. Most importantly removing duplicates.
- UNION ALL will give you data from both tables w/o removing duplicates.

# What is duplicate in sql ?
- Same data that has in 1 column. It is looking the entire row and entire result. 
- It is on the row level, not on the column level. Entire row level.

# MINUS in SQL ? 
- MINUS operator will remove those row from 1st table if it exists in table 2.

      FOR EX: TABLE 1 : Vanya , Lena , Jenya, Katty, John
      TABLE 2: Danny, Natalie , Vanya, Lena
      - TABLE 1 MINUS TABLE 2:
      Output: Jenya, Katty, John, Danny , Natalie

      2nd Example : TABLE 2 MINUS TABLE 1
      Output: Danny, Natalie, Jenya, Katty, John


# Tell me the difference between join and set operator ? 
- Set operator will combine the result of 2 query if they have same column count, column name, data type. Combine and return as 1 table.
- Joining 2 table with primary key and foreign key relationship in order to get the data that exists in both table.


# What are Table constraints ?
- Special rule that can be set. 
- Primary key
- Not null

# What is DML , DDL, DCL, Transaction Control ? 

- DML is Data Manipulation language. It is when we are doing some actions with created data. Like we are doing CRUD operations , and merge. Commands like : SELECT, INSERT, UPDATE, DELETE, MERGE.
- DDL - is Data definition language. We don't have access to it, but it is when we are creating , deleting. Commands like CREATE, ALTER, DROP, RENAME, TRUNCATE, COMMENT.
- DCL - Data control language. I never deal with it. As a tester I can't delete the table, that's what it means. Blocks some certain actions.
- Transaction Control - when multiple actions need to happen together. Either succeed or fail.

# How do you connect to the database using Java ? 
- By using JDBC. (Java Database Connectivity) JDBC. It is a bunch of interface that define the rule. It doesn't provide the implementation. 
- Who provides the implementation then ? The vendor. (Oracle, MySQL, etc)
- Then I need to connect the driver according what database I want to connect, then I start with using connection object, getting statement, writing the query, then getting resultSet object.

# Tell me exactly how do you connect to the database using Java line by line. 
- First I provide the driver (providing the dependency) , then the driver manager.getConnection, and I provide connection string, provide the username and password , and then get connection object

- Then I runQuery to get the ResultSet object :
```
ResultSet resultSet = statement.executeQuery("SELECT * FROM REGIONS")  ; 
```

- Then I use my methods in utilities. 

# Where have you used your database ? 
- In one of my project, I needed to add some data and test case was just about that , do the flow , add some data and make sure it works with success message according to the requirement. But production defect came out us, even tho we got success, the data was not added  into the database , the data was not persisted , the data still showed up , while user logged in, but it stops showing up , when user logged back again , basically it didn't show up in the database. But it did store in browser cache for whatever reason. So, in order to avoid that from happening , I write the test, If it didn't save into the database, just check if it did at that moment or not. So I write the query, get the expected result and compare that with the actual result. So it becomes the UI - DB validation. 

- Fix your data issue, get up to date data at all time to drive my test
- Save it as expected result to validate actual result.


