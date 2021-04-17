# _Java_

## 1 - What's the difference between HashMap and HashTable ?

- They are storing key-value pairs in a hash-table.

####

- HashMap : 
    - is non synchronized , not thread-safe 
    - accept null values 
    - more preferred over HashTable
    
- HashTable : 
    - is synchronized , thread safe
    - doesn't accept null values 
  
## 2 - Exception : checked vs unchecked

- Checked(Unwanted event)
  - Requires you to check it immediately! Expected. Like Thread.sleep...
  - Occurs during compile time... 
  - REQUIRES IMMEDIATE ATTENTION.
  - All exceptions that are not run time are checked exceptions
  
- Unchecked (Unexpected event)
  - Occurs during runtime
  - RunTimeException class is the parent of all Unchecked exception
  - All Runtime exceptions are Unchecked Exception

## 3 - Can you tell us the differences between List, Set, and Maps ?

- List : 
  - Has index. Accepts duplicates

- Set : 
  - Does NOT have index. Does not accept duplicates

- Map :
  - Data structure based on key+value pairs
  - Map interface does not extend Collection interface
  - It may contain duplicate values but keys are always unique.

## 4 - What is the length of the EMPTY and null string ?
- Null means nothing. It's just a literal.
- Null is the value of reference variable. But 
- Empty string is blank. It gives the length=0. 
- Empty string is a blank value, means the string does not have anything.

## 5 - What is the difference between collection and collections ?

-Collection : 
  - It is the interface where you group objects into a single unit. 
  - Does not have all static methods in it

Collections :
  - It is a utility class that has some set of operations you perform on Collection.
  - Collections consist of methods that are all static.



# _SQL_

## 6 - What is MetaData ?

- Data that provide information about other data.
- Think about the last time you searched Google. That search started with the metadata you had in your mind about something you wanted to find. 
- You may have begun with a word, phrase, meme, place name, slang or something else.

## 7 - Have you worked with non-relational databases ?
- I don’t have hands-on experience, but I know that it is there are no tables, rows, primary keys or foreign keys.
- examples of them : MongoDB, Apache Cassandra, Redis, Couchbase and Apache HBase.
- But if needed , I always ready to learn new stuff

## 8 - How can you find 3 HIGHEST PAID employees ?
- SELECT salary, first_name, last_name FROM employees ORDER  BY salary DESC LIMIT 3;

# _API_

## 9 - Do you know HTML Status Codes ?
- 200 Success
- 400 Users side error
- Server side error 

## 10 - What is EndPoint ?

# _Cucumber_

## 11 - Do you know any maven commands ?

    extra:
    12 - How to get the second max value in a table ?
