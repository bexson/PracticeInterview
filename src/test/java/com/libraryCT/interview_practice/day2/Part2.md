# 1. What is boundary testing?
#### ( CVS interview question )
   * Boundary testing - is type of testing, where tests are performed using the boundary values.

   
   * These boundary values can be either valid or invalid.
     - Assume, we have to test a field which accepts Age 18 – 56
     - Minimum boundary value is 18
     - Maximum boundary value is 56
     - Valid Inputs: 18,19,55,56
     - Invalid Inputs: 17 and 57
     - So in boundary value testing we test only the exact boundaries, rather than all the values



# 2. How to check if the master branch has your commit in git?
#### ( ARC Airlines )
- 1st way is : I would check out my master branch and use `git status` command, and if it says : `nothing to commit, working directory clean` , then I've pushed the current commit.

  --- or if it says : `On branch master. Your branch is ahead of 'origin/master' by 1 commit.` , then I have a local commit that has not yet been pushed. 
- 2nd way is :  I would go to git console and double click to remote master branch , so I will see all the commits on that remote origin/master branch , and if I see my commits on that branch , it means it has these commits. 
   
# 3. How do you produce the automation test result ? 

### ( ARC Airlines )

- Checking if automated tests are built correctly, i.e. are they testing what they were intended to test
- Reviewing individual test results and uncovering why failed tests failed
- Analyzing test results across the board to understand why some tests fail more frequently than others

# 4. How do you compare two values from different data structures?

### ( InfoSys )




# 5. Imagine that you are the test lead, and you have a security issue with the Login functionality. What would you do?

### ( Ebay ) 
 - I would ask PO about it


# 6. What are the 3 key things you and your scrum team ensure the piece of code you give a sign-off on that meets certain quality standards? 

### ( TCS/Amex ) 

In my team , code that is considered good:

- Does what it should.
- It is easy to understand.

- It can be tested
   
# 7. What is the difference between progression and regression testing? 
 
### ( TCS/Amex )

- Progression testing focuses on new functionality and proving that it works as per the requirements. Whereas regression testing focuses on proving that existing functions of the application are not broken from the addition of new code.

# 8. Imagine that you do not have enough time to test an application. What will you do: Do a quick test…? What will be your approach ?

### ( PNC bank )


# 9. You mentioned the cucumber BDD framework, there are two different types of cucumber BDD which one is yours?  
### ( BankOfAmerica )

 - I use Junit
   


# 10. Imagine if you have an API test case that is data-driven (id) and after you pushed the test case to GitHub -> Jenkins - it shows 503 status code. Why? Where do you see the status code?  

### ( Sogeti )

- 503 status code is about server side error. So it means the server is currently unable to handle the request coz it is overloaded or scheduled maintenance. I can see the status code using developer tools.