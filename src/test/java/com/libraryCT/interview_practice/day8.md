# API Questions

##### 1. How did you do API testing ? What was your purpose ( in my last project )
- I have experience both in Postman and RestAssured Library.  So , in Postman I was doing manual testing , and automation like verifying the status code  , checking the body , headers by using some basic knowledge of javascript , I was also able to run my collections from command line and getting the newman report. So , talking about RestAssured , I created the framework. I have conf.properties, utilities and basically I was doing a lot of assertions , so I tested the app functionality works in api layer.  


##### 2. Give us an example, step by step, how you would automate a test case API side. What do you do ?
- First I'd read the documentation (functional requirement) of the app , then understand what is each endpoint for , what of kind endpoints are available, what kind of authorization and authentication is needed , and is there any query , path params that I need to provide to send the request and what I am expecting according to such information that I provide in each request. 

- So when I have this understanding , I use Postman to get all kind of diff result , so that , I can write my test cases around those scenarios and automate them right in postman. 
  
- Or I can create a RestAssured project to automate my test cases, like building up my utilities (according to whatever app I am working with ), and use junit5, and start automating it from there according to the test scenario or diff test result that I saw.

##### 3. Give an example on an API test you recently wrote and how detailed you went with the test case ?

- In a recent POST /add_user endpoint , 
- It expects a json as payload, and it has strict restriction on the field values like name length , phone number , email verifications , the right status along with the positive scenario where I add correct json payload and expect 201 status code with valid headers and response payload 

- I added negative scenarios for all kind of 400 BAD REQUEST scenarios, 

- like either name as invalid length , phone or email has invalid format , status is not right or multiple invalid inputs
- I have added additional GET /get_user_by_id/{id} requests to verify the data was actually added correctly
- Same flow repeated for PUT and PATCH Requests

##### 4. How do you validate a JSON payload ?
- I can do validation of json body both in Postman and RestAssured. 
    - In postman , I save the json response as JavaScript object and access the property of the object for verification.
    - In RestAssured , I use JsonPath to capture the value of the field to be verified and compare that with expected result in the test.

##### 5. How would you validate only part of the body of a response ?
- I would capture the value from the json , using method from JsonPath object and compare that to according to the expected result. 

- I also add additional validation for JsonSchema to make sure the json structure is as expected according to the requirement.

##### How would you test the structure of your Json Response without having to verify the actual value of the field ?
- I do JsonSchema Validation to verify the structure of the json response. I have JsonSchema file that I got from developers to describe how the response json structure should look like.
          
      one example : get("/products")
                    .then()
                    .assertThat()
                    .body(matchesJsonSchemaInClasspath("products-schema.json"));

##### 6. How can you convert from Json to Java Object and Java Object to Json ?
- Serialization : Java Object to Json
- Deserialization : Json to Java

- I have POJO(Plain Old Java Object) class that represent the structure of json object I use Jackson Data-bind library to do such conversion known as Serialization and De-Serialization

- POJO Class is used to represent data , it does not have extra functionality,  other than representing data
    - It should have: 
      - Encapsulated fields (private fields , public getters and setters)
      - No Arg Constructor (REQUIRED)

##### 7. Describe where else did you use API other than API Testing ?
Some of my UI scenario heavily rely on the correct data in correct state to be able to go through application flow. I did not have access to database or getting data from database was too complex since the data was spread among too many different database tables. However, there was api endpoint that return such data I am looking for easily. So I made api call to get my test data and pass it to UI Scenario to drive my UI test. In some other scenario I used to for generating test data easily and fast.

##### 8. Have you worked with XML response ?
- Not recently , Most of the API Endpoint I have worked on return Json response. I can work with XML Response using XmlPath in RestAssured

##### 9. How do you test business restrictions that are on the API ?
- Restriction can be multiple things ,like restriction on authorization and authentication or restriction on valid data while adding data orr updating data. Use multiple different test scenarios to test positive negative scenarios according to the restrictions. 

##### 10. How would you test the structure of your Json Response without having to verify the actual value of the field ?
- I do JsonSchema Validation to verify the structure of the json response. I have JsonSchema file that I got from developers to describe how the response json structure should look like In RestAssured Project I have below dependency
