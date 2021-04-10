<!-- Headings -->
#Soft - Skill
##1-What is the difference between STLC and SDLC ?##
*  SDLC is a Development Life Cycle whereas STLC is a Testing Life Cycle.
- STLC is mainly related to software testing.
- It focuses only on testing the software.
- In STLC, testing team makes the plans and designs.
- Goal of STLC is to complete successful testing of software.
---------------------------------------------------------
- SDLC is mainly related to software development.
- Besides, development other phases like testing is also included.
- In SDLC, development team makes the plans and designs.
- Goal of SDLC is to complete successful development of software.

###2 - When Should The Testing Start?

- It should start since the beginning of SDLC with testing the requirement.
- We have to make sure the requirement is correct in the first place. 
With the wrong requirement it is impossible to build a bug free application.
  
###3-What is a tester’s main responsibility?
- To find bugs as early as possible. Make sure most of the bug gets fixed. 
- To satisfy the end user and client by delivering a bug free and user-friendly application. 

###4-What is the testing hierarchy?
- Unit testing:Developers test each module or block of code during development. 
- Component Testing : Component is a standalone functionality that can work by itself. 
  - Ex. Amazon Buyer Functionality, Seller Functionality, Prime Video Functionality. 
- 3.Integration Testing: Combine all the functionalities. When I integrate them, can I still use all the functions? Make sure they all still work.
- 4.System Testing:End-to-End testing. Test everything from beginning to end. 
- 5.Acceptance Testing: Hire a UAT (User Acceptance Testing) Team or Business Analyst can also do Acceptance Testing.
 After testing has been completed you have to get another team to do acceptance testing, so they can confirm the QA teams testing was successful and have the product ready for the customer.

###5-What is Functional Testing?
- The purpose of Functional tests is to test each function of the software application, by providing appropriate input, verifying the output against the Functional requirements.
- mainly involves black box testing and it is not concerned about the source code of the application.

#Java
###1 - What are the access modifiers?
- Public: accessible from everywhere 
- Protected: accessible within the same package or subclasses in different packages. 
- No modifier/default: accessible only within the same package. 
- Private: accessible only within the class.

*I use private access modifiers to achieve encapsulation to limit the outside access. I make the constructor private to avoid class instantiation as in the Driver class. All fields in POJO classes are private.*

###2-Pass-by-Value vs Pass-by-Reference
- I have no idea what is it

###3-Final vs finally vs finalize()
- Final: it is a keyword and used to apply restrictions on class, method, and variable. 
  - Final Class = CAN’T be inherited 
  - Final Method = CAN’T be overridden
  - Final Variable = CAN’T be changed 
- Finally: it is used for exception handling with try and catch block. 
  - It is executed every time even if an exception happens or not.
  
*In my project , I used it in DB_Utility , to return cursor : rs.beforeFirst*
###4-Where did you use static in your framework?
- in BrowserUtils class where I use static to call method just using classname , instead of creating an object of it
- in ConfigurationReader class
- in Driver class , when I create an object of ThreadLocal to have 1 copy
###5-Difference between equals method and “==” operator in Java ?
- Equals with strings 
- == operator for numbers