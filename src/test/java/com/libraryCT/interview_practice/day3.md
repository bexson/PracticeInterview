# Soft - Skills

##  1 - What is Verification and Validation ?

 1)  Verification process - it is a process of ensuring we are developing the product according to specifications.
     Does NOT involve code or project
     
     - It goes through 3 meetings :
       1. Review
       2. Walkthrough
       3. Inspection
 

2)  Validation process - it is a process of testing and validating the actual product to ensure we have developed it correctly.
  
    So it is kinda computer-based testing code. 


# 2 - What is Smoke Test ?

#### Smoke test is a type of testing to check if the application up and running. I'm doing it every day morning before start to work using Jenkins. 
 - extra things to remember about Smoke Test : 
    - takes around 15~20 minutes to run
    - around 6~8 user stories here in total

# 3 - Regression Testing ?

#### -  It is a type of testing to verify that software previously developed modules are still working with the new added module 
#### or to make sure that a product still functions after code changes or updates. So in my team we are doing it each time before release. 
- extra things to remember about Regression Test :
  
    - Why ? To check if the new functionality works with the old ones
    - When ? Before release or at the end of each sprint 
    - US in total ? It depends.   (400~1000) 
    - How long it takes to run ? It depends. It takes around 30 minutes to run. 
    - We have around 500 test cases.
    
# 4 - What is a defect ?
- When the expected result does not match the actual result, it is a defect. 

# 5 - What is Defect Life Cycle (DLC) ?
- It is a lets say a journey of the defect from its identification to its closure. 
- extra things :  New --->  Assigned ---> Open ---> Fixed ---> Retested ---> Close

# Java

## 1 - What is Singleton class and how can we make a class Singleton ?
- It is a class that can have only one object (an instance of the class) at a time. After first time, if we try to instantiate the Singleton class, the new variable also points to the first instance created.
- We need to have static member of class, private constructor and static factory method.  
                                
        - extra things :  
        Static member: It gets memory only once because of static, it contains the instance of the Singleton class.
  
        Private constructor: It will prevent to instantiate the Singleton class from outside the class.
  
        Static factory method: This provides the global point of access to the Singleton object and returns the instance to the caller.

# 2 - What is String Pool in Java ?
- String Pool in Java corresponds to an allocation of memory in Java heap memory.
- extra things to remember :
    - It's located in the heap
    - It will store the literal objects --> It will have same memory for objects that have similar values
    - so there will be no duplicate values

# 3 - Difference between overloading and overriding ?
- Method overloading : 
    - is performed within class.
    - it is multiple methods with same name, but different parameters
    - any method can be overloaded
    - extra : example of compile time polymorphism.
- Method overriding : 
    - it is one method with different implementation
    - we cannot override static, final, private methods
    - access modifier MUST be same or more visible
    - return type, method name, parameters MUSt be same
    - MUST happen in subclass
    - **__extra :__** example of run time polymorphism
    
# 4 - Abstract Class and/vs Interface ?
#### Both used for achieving abstraction , meant to be inherited ( extends, implements) , cannot be final , cannot create objects
- Abstract class : 
    - a class can only extend one abstract class
    - can have everything a regular class can + abstract method

- Interface : 
    - a class can implement multiple interfaces
    - in interface variable by default is public static and final
    - methods by default abstract, can have static , default methods