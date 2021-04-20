# SDLC
#### 1-Is 100% testing possible ?
- We can’t test the application 100% since there are unlimited scenarios that we can’t even imagine. 
- The application is dynamic and developing in time so the new functionalities will require testing.
  
- (another answer : 100% bug free testing is not at all possible. If we say 100% testing is completed, then that will be the end to any software. Then why we are getting so many projects still. Because we didn't develop a bug free project. We can't develop a bug free project).

#### 2-What is Agile Methodology ?
- It is software development methodology , where people work together as one team to reach client's satisfaction

- More human communication, interaction happening here 

- Users give continuous feedback for an app

- Mostly in IT , companies are using Agile , since welcome changes , team work , deliver frequent, self-organizing teams 

#### 3-What is Feature ?

- Feature is multiple user stories that you can put together, and it becomes a stand-alone component of one application.

        example : As an Amazon Prime member I should be able to stream movies online, so I don’t have to use Netflix.
    
        It is not totally away from amazon, it is under amazon project, but it can be stand alone component of amazon.com
        
#### 4-What is a User Story ?

- It is basically just a requirement.

- User story is a short simple description of a minimum shippable product. 

- It normally looks like this: As someone , I should be able to do something. 

#### 5-What is an Acceptance Criteria ?

- Acceptance Criteria - is the way that we know the user story is successfully developed or not. 
- When BA or PO write user stories, s/he writes AC together.

       another answer - Acceptance criteria (AC) are the conditions that a software product must meet to be accepted by a user, a customer, or other system. They are unique for each user story and define the feature behavior from the end-user’s perspective. Well-written acceptance criteria help avoid unexpected results in the end of a development stage and ensure that all stakeholders and users are satisfied with what they get.

#### 6-What is Rat hole and Parking Lot Item ?

- Rat Hole - it is in the meeting when the team gets into too much argument and wasting time we call it Rat hole. As soon as someone says it is Rat hole we should stop arguing.

- Parking lot item - it is a valid problem in the meeting, but it is your specific problem, so if you keep people discussing your problem in the meeting because we are wasting other people’s time.
 - < "Let’s make it a parking lot item" > means whoever is interested in that issue can talk after the meeting.

# Selenium
#### 1-What is the difference between “relative” and “absolute” XPath ?

- Absolute xpath - it is not stable ,  NOT RECOMMENDED TO USE ,  because we are starting from the root element html , and we go 1 by 1 from parent to child until we reach to the desired web element.
  - it starts with single / slash 
  - It will break if there is any slight change in the web element structure.


- Relative xpath
  - starts with double slash "//"
  - Double slash means we can start from anywhere in the page.
  - It is a lot more reliable than absolute xpath because we are being a lot more specific.
  - We can locate a parent and go to child.
  - We can locate a child and go to parent with xpath.
  
#### 2-How can we move to the nth child element using Xpath ?

- by using square brackets with index position 
    - div[2] it will find 2 nd div element 
  

  

#### 3-How Can We Move To The Parent Element Using Xpath ?
- we should use /..

#### 4-What is Xpath ?
- One of the 8 locators , which I'm using most of the time
- It is used to find the location of any element on a webpage using html structure.

#### 5-Difference Between close() and quit() command ?
 - close():  closes the currently opened page(browser)

- quit(): used to quit the whole browser session along with all the associated browser windows, tabs and pop-ups.

#### 6-Difference Between Xpath And Css Selector ?
- first difference is syntax 
   - css : div[class='ad99']
  - xpath : //div[@class='ad99']

- Xpath can search elements backward or forward while css works only in forward direction.
- Xpath can work with text, css cannot work.
- Xpath has more combinations and can search by index, css cannot search by index
- CSS is faster than XPath, but I never experienced it in my framework as it is a smaller project.

#### 7-Implicit / Explicit / Fluent Wait ?
- Implicit wait :
  - We set it up ONLY ONCE.
  - it applies to every line we locate a web element.
  - By default, it has value of 0.
  - This will be triggered when driver is not able to find WebElement.
  - We can increase the number of wait time by changing the value.
  - It will wait for the given duration.
  - Then if not found, it will throw NoSuchElementException. 
  - (- If the wait time set for 10 seconds, but the element found in 3, the remaining 7 seconds are not waited in both implicit and explicit wait)
  
#####
  
- Explicit wait : 
  - When we need to wait for a specific condition to happen we use Explicit waits.
  - It is smart wait, meaning, it will wait UP TO given seconds.
  - But if the condition happens before the time is up, it will continue.
    
  - To implement, we need to create instance of WebDriverWait class.
  - In the constructor we pass: Driver instance, and TimeOutSeconds
  

#### 8-What is “Thread.sleep()” ?
- Comes from Java library.
- This is 100% full java code.
- No relation to Selenium what so ever.
- What this line does; it literally stops the whole execution of the java program.

- We use it occasionally to allow the browser to catch up with the browser driver.

#### 9-Why and how to locate elements using “text” ?
- There might be cases where no locator is available to find an element, so you may need to use text().
  
- For example, you’re trying to find the “sign in” button but there is no id, class, etc. available, so you can just search
  for the text “sign in” which is written on the button. In this case, Selenium will look for the text to locate it.

#### 10 - How to handle select drop down menus ?
- we need to create a new object out of select class which has already been blueprinted by Selenium developers.
- Import Select Class and create an object. This new object will come with its own methods like select ByValue, select ByIndex, etc.

- If there is a select tagName , it means that 99% it is a select dropdown.


# Extra:
#### 1-What are the advantages of Selenium ?
- Selenium is open source and free to use tool. 
- It supports multiple languages like Java, Ruby, Python, C#.
- It supports multi-browser testing
- It has a good amount of resources and a supporting community.
- It supports many operating systems like Windows, Mac, Linux ...
- It interacts with the web applications

#### 2-What are the limitations and disadvantages of Selenium ?
- Selenium supports only web-based applications , does not support windows based application 
- No built-in reporting tool, it needs third party tools for report generation activity 
- Cannot work with graphics, captcha, barcodes, shapes 
- It does not support file upload facility. 
- Hard to write good and stable locators since they are dependent on web developers. 
- We have to use external libraries and tools for performing tasks like testing framework (TestNG, JUnit), reading from external files (Apache POI for Excel)
#### 3-What is automation and what are the benefits ?
- Using software or computers to automate manually done actions. 
- It helps you save money and improves efficiency. 
- It is faster and safer since there will be no human error. 
- You can run it anytime, anywhere, 24 hours. 
- Test automation is automating the testing process using specific software. This requires new sets of skills and using tools like Selenium, cucumber, Serenity, UFT, appium, Protractor, etc. 