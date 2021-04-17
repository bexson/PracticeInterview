## 1. What is TestNG ?
- It is advanced unit testing tool that allows us creating test flow using annotations.
####
- Originally it was created by a developer for developers.
- It is created based on JUnit.
- As SDET I use it to create certain test flow with its annotations such as:
  - BeforeMethod, AfterMethod, BeforeClass, AfterClass...
####
        extra : 
        annotations: @Test , @BeforeClass/@AfterClass ,
        @BeforeMethod/@AfterMethod
        @Test annotation helps us create TestNG tests where we can implement Java+Selenium code and use Assertions coming from TestNG.	
        ASSERTIONS :     assertEquals , assertTrue, assertNotEquals

## 2. Difference between JUnit and TestNG ?

- Both are Testing frameworks which help us to run automation scripts.
- 
- TestNG is inspired by JUnit.
- Small differences in annotations names , but most of them are doing same things.
- TestNG is more powerful than JUnit since few more functionalities are added to it. (I will just say like this, but I don't know what are functionalities)

      extra: 
      TestNG has @Dataprovider annotation same as Cucumber Scenario Outline for Data Driven Testing.
      TestNG and JUnit both of them have parameterized testing but TestNG parameterized test configuration is very easy to configure. There are two ways to achieve parameterization in TestNG; ➢@Parameters and TestNG xml file ➢@DataPrivider

## 3. What first thing you check when you get response in API ?
- I would first check status , just to make sure, if I get right status(200) , then I will get right data, which I will work on. 

## 4. Parameters in API ?
- Query Parameter :
  - A key value pair. Usually used to filter the result
  - It's easily recognizable in the url because it always comes at the end of URL right after ?
  - It can also be used for providing the api keys in some api
  - It can be used for specifying the response content type if the api doc says so

####

- Path Variable or Parameter : 
  - Used to identify single resource among list of resources
  - It's part or url directly
  - Usually clearly defined in the doc either use :name or {name} (colon , braces)

## 5. Authorization vs Authentication ?

- Authentication : Telling the system who you are , proving the identity against whom you say you are.
- Authorization : Things you can do according to who you are, The permission attached to your identity.

## 6. What kinds processes can be automated using jenkins ?
- There can be automated smoke tests , using maven command
- Regression testing 

## 7. What is the difference between integration test and end-to-end test ?
- Integration testing : 
  - Integration testing starts at the very early stages of development. Bugs are caught earlier, rather than later, in the cycle.
  - It's easy to integrate with daily builds and easy to test in the development environment.
  - Tests run faster compared to end-to-end tests.


- End-To-End Testing : 
  - End-to-end testing is done when the product is almost ready for release.
  - It may be impossible to perform until the product is nearing completion.
  - Tests run slower compared to integration testing.
  
## 8. Can you talk about your team structure ?
- There are 13 ppl, 5 devs and 3 testers
## 9. Let’s say you’re given some test cases; how do you decide them to automate or not? Can you tell me any specific factors?

## 10. How does your Jenkins sends the reports? How do you store the reports ? What kind of reports do you using?

- I'm getting reports from Jenkins by email. When cucumber - reports for automation , they are storing
maven cucumber reporting 

when setting up Build I chose cucumber reports. It's being store by jenkins in the devise that is running smoke test,
also Jenkins stores reports in XML files in the Jenkins home directory. Here also all the build history is stored. 