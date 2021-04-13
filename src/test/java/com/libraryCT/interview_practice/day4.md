# API Questions 

## 1 - What is an API ?

##### API - it is a small piece of code that enables different applications and services to communicate and share information with each other. 

##### extra info :
##### There are 2 types of API : 
- SOAP ( Simple Object Access Protocol)
- REST(Representational State of Transfer) 

## 2 - What is API Testing ?

##### API Testing is - a type of software testing that involves testing APIs directly. API testing is entirely different from GUI testing and mainly concentrates on the business logic layer of the software architecture. This testing won't concentrate on the look and feel of an application. 

    ___extra____: Instead of using standard user inputs and outputs, in API Testing, we use software to send calls to the API, get output, and note down the system's response.

    API Testing requires an application to interact with API. In order to test an API, you will need to: 
    1. Use Testing Tool to drive the API
    2. Write your own code to test the API

## 3 - What are main differences between API and Web Service ?

- All Web services are APIs but not all APIs are Web services
- Web services might not contain all the specifications and cannot perform all the tasks that APIs would perform.
- A Web service uses only three styles of use: SOAP, REST and XML-RPC for communication whereas API may be exposed to in multiple ways.
- A Web service always needs a network to operate while APIs don’t need a network for operation.

## 4 - What are the advantages of API Testing ?
- API testing provides access to the application without a user interface. 
- Time Effective : so API testing is less time-consuming than functional GUI testing
- Language-Independent : In this testing, data is exchanged using XML or JSON. It, allowing users to select any code language when adopting automation testing
- Easy Integration with GUI: API tests enable highly integrable tests, which is particularly useful if you want to perform functional GUI tests after API testing. For instance, simple integration would allow new user accounts to be created within the application before a GUI test started.

## 5 - How do you make assertions while doing API testing ? Which assertion dependency are you using for that?
#### ( InfoSys )

- So , in my project, for Postman, I'm using assertions from Chai Assertion Library by implementing some basic javascript knowledge. And so , talking about RestAssured - most of the time I'm using hamcrest matchers by the help of Hamcrest Matchers Library, it just makes the assertions more readable , and  also sometimes I use assertions from junit-jupiter library like assertAll.

## 6 - How do you write restful API in JUnit 5 ? Where you write headers, request type, headers, query parameters, and respond validations ? (InfoSys)

- 

## 7 - What is URI and its purpose in terms of API ?

- URI - is a sequence of characters that identifies a web resource by location, name, or both in the World Wide Web. It is a method that allows for the uniform identification of the resources. So the main purpose is to find a resource and differentiate it from other resources using either name or location.

## 8 - What type of Authentication are there in API? What is an OAuth ? What is JWT ?
- There are 4 types of them : 
   - Basic Auth
   - API Keys
   - Bearer token
   - oAuth2
    
- OAuth is a much more secure way of authorizing your request. 
- OAuth doesn't share password data but instead uses authorization tokens to prove an identity between consumers and service providers.

- JWT ? it stands for JSON Web Token. It is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.





## 9 - How do you use Collection in API testing ? (PK Global)
- I'm using collection when I should get list of info , and by the help of method getList from json path , I get the list of IDs for instance.


## 10 - Can you give me scenario how do you do API testing ?


            extra
    (#### 9 - Why are we called restful services, what is the difference from SOAP ? )
    What CRUD operations do you know in API ? ()