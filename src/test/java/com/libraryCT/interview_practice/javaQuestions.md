# Java Questions & My answers 
 
## 1 - What would you rate your Java experience out of 10 ?

##### ---> I would rate 7 out of 10.

## 2 - What is your java level ? Do you use it in terms of testing only or in terms of development as well ?

##### ---> I use it in terms of testing and development as well. Since I can add any function to my framework 

## 3 - OOP concepts and how you used them in your last project ? 

##### --->  Actually , I used Encapsulation, Inheritance ,  Abstraction, Polymorphism  

- Encapsulation - used to hide the data by using private keyword and generating public getters and setters.
  - In my Serenity - RestAssured framework I used it in POJO classes by using getters and setters , and making variables as private.
  - In my UI framework
    - I used it in the Driver class by making constructor as private and generating public getter for driver.
    - Also, I made as private the Properties object and generated public getProperty method.
  
- Inheritance - is used to create parent/child relations. 
  - In my UI framework I used BasePage - so, it is parent class for all the Pages , and we extend BasePage into other Page classes, and we inherit parent class constructor as well , so that we don't need to initElements in subclasses (Page classes)
      - initElements();
    
  - If I use TestNG ,in TestBase class I use methods such as setUp , tearDown for all common classes
  
- Abstraction - used to hide the implementation details. So we focus on essentials.
  So there can be 2 ways to achieve abstraction : interface or abstract class
  - in my framework I use interfaces such as 
    - WebElement , WebDriver , JavaScriptExecutor , Wait , Connection, Statement, ResultSet
    List, Set;

- Polymorphism - it is the ability of the object to take on many forms. (means "many forms")
  - in my framework I used WebDriver as referenced type and all types of browsers, such as chrome, firefox I used as object type.
    - So, that regardless what type of browser I use at the end I can return any type of driver like chromeDriver, firefoxDriver.
    - Also, I used List as reference type and ArrayList as an object type.

## 4 - What do you know about Interface  ?

##### --->  So, it is one of the way to achieve pure abstraction. One class can extend multiple interfaces.
##### --->  We can have multiple inheritance. One class can implement multiple interfaces.  
##### --->  Variables are public static and final by default , methods are public and abstract by default , we can have static or default methods
##### --->  we can't have : objects , constructor, instance methods, instances(only in the class, in the objects), blocks

## 5 - What is the benefit of interface ?

##### --->  It allows us to have multiple inheritance. One class can extend multiple interfaces.

## 6 -  What kind of collections you used in Java ?

##### --->  Collection is one of the data structures in Java. (Array, Collection , Maps )

- I used List , Map;
- I used List to store WebElements. Or I have dataTable, and I store all the data's in the List.  
- for Set, I stored only unique windows or if I need to store elements from dropdown box I prefer Set to have unique ones.
- I used in API testing Map, like if I create a librarian , I should use Map to store data's in key and value format.

## 7 - How to call the last stored variable in an Array ?

##### --->  I can use length-1 

## 8 - Where do you use Set, HashMap, List in your framework ?

##### --->  I used set to store only unique tabs/windows, or if I need to store elements from dropdown box I prefer Set to have unique ones.
##### --->  I used HashMap when I get data from 2 columns in datatable in Cucumber framework. Or when I get data from Json response
##### --->  I used List to store WebElements. Or I have dataTable, and I store all the data's in the List..
##### --->  List : has duplicates , index, Set doesn't have index , doesn't accept duplicates

## 9 -  What is the difference between iterator and for/for each loop ?

##### --->  Iterator applicable only to the objects that having IS A relation. That's why we can use iterator for Collections  
##### --->  For Each loop we can use for anything
##### --->  For ex if we have arrayList: with Iterator we can remove any element, but with ForEach loop we can't
##### --->  ForEach applicable everywhere 

## 10 -  What iterator methods do you use ?

##### ---> iterator(); - will iterate 
##### ---> hasNext(); - check if there is any more indexes
##### ---> next(); iterator
##### ---> remove(); 

## 11 - How do you write or read data from or to file with Java ?

##### ---> In order to read and write I used BufferReader and BufferWriter.
    extra: Or I can use Properties object 
    And Also I can use Scanner and while loop 

## 12 - Difference between Heap and Stack ?

##### ---> Heap we use for object and instances
##### ---> All local variables will be stored in Stack.
    stack is the memory location for primitive values that are specific to a method
    and references to objects that are in a heap, referred from the method.

## 13 - You have a list of fruits which some of them repeats. How would you write a method which will return a fruit that repeats the most ? ?

##### ---> I would find the frequency of each fruit by using Collection.frequency() and find the max frequency


## 14 - Java version you are using? 

##### ---> I'm using java 8

## 15 - Abstract class vs Interface?  

##### ---> Abstract is class , Interface is blueprint of the class
##### ---> in abstract class we can have constructor , instance methods, variables, however in interface we can't
##### ---> Interface can have multiple inheritance
##### ---> In interface we can have only public access modifier, however in abstract class we can have any
##### ---> Different keywords: extends for abstract class, implement for interface


## 16 - Java generics (Java types) ?

##### ---> Java generics are java types.
##### ---> When we don't specify type, we can store any type. 
##### ---> List list = new ArrayList();


## 17 - What is HashMap explain, how do you use in your framework ?

##### ---> HashMap is used as a pair of data. The keys are in random order. I'm storing it sometimes if I have datatable.

##### ---> When I'm implementing serialization and deserialization, when I'm getting the data from Json, properties type of file.

## 18 - What is thread safe ? How do you make your code thread safe ?

##### ---> Thread safe means 1 thread at a time. Thread - is subsequence of the process.

##### ---> I can make my code as thread-safe by using synchronized keyword. And I can apply it for methods, blocks.
##### -> in my project I created the “getDriver()” method in Driver class as thread safe because I don't want the Driver to be called simultaneously.

## 19 - String builder/buffer differences ?
- both are mutable, changeable
##### ---> StringBuilder - is un-synchronized , not thread-safe
##### ---> StringBuffer  - is synchronized , thread-safe -> slower performance

## 20 - How can you achieve abstraction ?
##### there are 2 ways : 

##### ---> abstraction class. 
  - not concrete , can't create an object
  - WE USE IT WHEN WE WANT TO CREATE A SUPER CLASS

##### ---> interface
  - not a class, blueprint of the class
  - can't create an object. 
  - ALL variables are public static by default
  - we can have STATIC METHODS 
  - IT IS FOR PURE ABSTRACTION
  - WE USE IT, WHEN NOT ALL SUBCLASSES NEEDED , BUT SOME OF THEM MAY NEED

## 21 - What is the difference between List, Set, Queue ?

##### ---> LIST (Interface) : accepts duplicates , has index nums

##### ---> Set (Interface) : doesn't accept duplicates , doesn't have index nums 

##### ---> Queue(Interface) : accept duplicates , doesn't have index nums

- we have special order FIFO, poll() method will remove 1st element.

## 22 - What is Map ? 

##### ---> Map - is the data structure , where we store data in key&value format. 

## 23 - How do you iterate over HashMap ? 

##### ---> for iterating only the values I can use map.values() method and forEach loop
##### ---> for iterating only the keys I can use map.keySet() method and forEach loop
##### ---> for iterating both keys and values I can use map.entrySet() method and forEach loop

## 24 - What is garbage ?

##### ---> Garbage is not used object. Garbage's are eligible for garbage collector.

##### ---> If there is an object that is not having any reference then it is eligible for garbage collector, and he is going to collect them. 

- example of unreferenced object :
              
      ArrayList<Integer> list=new ArrayList<>(Arrays.asList(1,2,3,4,5)); // this object will be collected by garbage collector
      list = new ArrayList<>();
      
      int x = null;


## 25 - What is class in Java ? Difference between class and object ?

##### ---> Class - template of the object. We can have > 1 object in the class.

[comment]: <> (example of the class)
```java
public class Main {
  int x = 5;
}
```

##### ---> Object - blueprint of the class. Object can't exist w/o a class.

[comment]: <> (example of the object)
```java
public class Main {
  int x = 5;

  public static void main(String[] args) {
    Main myObj = new Main(); // object
    System.out.println(myObj.x);
  }
}
```

## 26 - What kind of exception you faced and how you handled ? 

##### ---> in UI framework I faced unchecked exceptions such as : 
- NoSuchElementException : I usually face this exception which usually happens because of synchronization issues, incorrect locators, or hidden elements in iFrame. 
- StaleElementException : It usually happens when the element has been deleted entirely. This is how I handle it: 1.Refresh the page and try again for the same element. 2.Wait for the element till it gets available.


## 27 - What is the difference between a HashMap and HashTable ?

##### ---> HashMap -  un-synchronized , not thread - safe, accepts null
##### ---> HashTable - synchronized , thread - safe, doesn't accept null

## 28 - What is polymorphism ? What is runtime polymorphism ?

##### ---> Polymorphism is the ability to take on many forms. 

##### ---> Runtime polymorphism it is a process in which a call to an overridden method is resolved at runtime rather than compile-time. In this process, an overridden method is called through the reference variable of a superclass.
    example of runtime polymorphism
    WebDriver driver = new ChromeDriver(); 
    driver.get(URL);
    .get() method will be called from the ChromeDriver(); since it is overriden in ChromeDriver class. 

##### ---> So, in Polymorphism the overridden method will always be executed.  

## 29 - Give me an example from your framework where you used OOP concepts ?

##### ---> Encapsulation : is used to hiding the data by using private keyword and generating getters and setters.
==> in my project ***: 
  -   RestAssured framework : POJO class by using lombok: private instance variables and public getters and setters
  -   UI framework : 
      - Driver class - private constructor and public getter
      - ConfigurationReader - private object of Properties and public getProperty method(getter)

##### ---> Inheritance : is used to create IS A relation ( super/sub || parent/child )
==> in my project ***:
  - UI framework : BasePage -  parent class , we extend BasePage into other Page classes, and we inherit parent class constructor as well , so that we don't need to initElements in subclasses (Page classes)
  - TestNG framework : I use in TestBase methods such as setUp , tearDown for all common classes. So I inherit TestBase with all common functions for all subclasses

##### ---> Abstraction : it is used to hide the implementation details. we focus on essentials.

==> in my project ***:
- interfaces such as : WebElement , WebDriver , JavaScriptExecutor , Wait , Connection, Statement, ResultSet, List<>, Set<>;


##### ---> Polymorphism : it is the ability of the object to take on many forms.
==> in my project ***: 
- WebDriver driver = new FireFoxDriver();
- driver.get(URL); --> The .get() comes from the WebDriver class, but the implementation comes from the object FireFoxDriver() class.

## 30 - What is global variable ? 

##### ---> It is static variable. Because it is acceptable in any place in the class.

##### ---> for ex: I can call static variable in instance method, but I can't call instance variable inside static method or block .  

##### ---> even I can call static member without creating an object.

## 31 - How do you handle exceptions ?

##### ---> try & catch - permanent solution, used for handling checked and unchecked exceptions
- all exceptions that are not run time are checked exceptions

##### ---> throws - the quickest solution, used for temporary solution , but not permanent solution, used for handling checked exceptions

    for example: 
    I created and handled sleep custom method , which will wait like Thread.sleep, but instead of giving milliseconds I'm giving seconds and handled it by using try&catch block, so that I don't need to deal with it in other classes.


## 32 - Difference between protected and default?
##### ---> protected - visible in same package and subclasses
##### ---> default - only inside same package.

## 33 - Can you give public: access modifier where you are overriding a protected method ?
##### ---> Yes. because for method overriding we can use access modifier same or > visible

##### ---> We can't override private, static , final methods.  
##### ---> Static => because when we override we are going to give multiple copies, but static make it to give 1 copy
##### ---> Final => because final means constant, so implementation can't be changed, however for overriding we are going to give different implementations.


## 34 - How can you find max value in an int array ?
##### ---> I can create int variable which I will use as max value and use for/each loop to compare 1 element till last element and whichever is largest I will assign to var max.

## 35 - Can class be final ?

##### ---> If the class is super class it can't be final. -> abstract class can't be final. So, other classes can be final if they don't have any subclasses. 
    extra : once the method is final, you can't override it.


## 36 - Static methods ?

##### ---> static method belongs to the class. We can call it through the class name

##### ---> in my framework: getDriver() , getProperty(); all methods in utils.

## 36 - Static, non-static methods ?

##### ---> non - static method belongs to the object. We can't call through the class name.

##### ---> I can use any variable in non-static method. Only the instance methods can be overridden.

## 37 - What is the difference between exception and the error ? 

##### ---> Error class represents critical conditions that can not be caught and handled by the code of the program. On the other hand, the Exception class represents concerning conditions raised by the application itself; these can be caught and handled within the code to ensure that the application continues to run smoothly.
# Errors : java.lang.StackOverflowError, java.lang.OutOfMemoryError
# Exceptions : NoSuchElement, SQLException, ArrayOutOfBoundsException


## 38 -
##### --->
## 39 -
##### --->
## 40 -
##### --->
## 41 -
##### --->
##### --->
## 42 -
##### --->
##### --->
## 43 -
##### --->
##### --->
## 44 -
##### --->
## 45 -
##### --->
##### --->
## 46 -
##### --->
##### --->
## 47 -
##### --->
##### --->
## 48 -
##### --->
##### --->
## 49 -
##### --->
##### --->
## 50 -
##### --->
##### --->
##### --->
##### --->
##### ---> 
##### ---> 
##### ---> 
##### ---> 
##### ---> 

