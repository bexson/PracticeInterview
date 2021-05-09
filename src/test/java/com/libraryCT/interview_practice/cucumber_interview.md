# What is Feature ? 
- Agile stories, user stories

# What is a scenario ? 
- Scenario - is basically our test cases. So we write a scenario as a test case. Which has the steps, and we use Gherkin language to do so.
- Scenario - Each test case we create from the user story.

- For scenario, we can give the tag. 
- Scenarios we use for the reporting. So it is also solving one of the problem. 
- For each scenario I will create a step definitions. 

# Cucumber CukesRunner 
- Plugins keyword : plugin keyword allows us to generate different types of test reports coming from cucumber.
- one of the simple report types coming from cucumber is "html report"
  - How do we implement?
    - Add the below plugin into @CucumberOptions
    - syntax: plugin = "html:target/cucumber-report.html"
    - "html" keyword is the type of the report
    - :target/  --> in what folder we want to store this report
    - cucumber-report.html --> what name we want to give to this report    

    
- Features keyword : We specify the location of feature files
- Glue keyword: We specify the location of the step-definitions 
- DryRun : is a way of actually running the code or just getting the snippets to implement.
    - if dryRun is true, it will NOT RUN ANY STEP DEFINITIONS CODE.
    - we turn it to true, when we don't want to run the tests, but we just want to get the unimplemented steps
    - we need to turn dryRun value to FALSE, in order to be ABLE TO RUN THE TESTS.
    
# What is snippet ? 
- unimplemented step definition methods

# In what order cucumber runs ?
- Cucumber runs from the feature files steps order.
- The order in step_definitions does not matter.
- Only the order in the .feature file steps matters.

# Step by step how to create a scenario and implement it ?

 1) Create a feature file. Named something.feature --> Extension must be .feature
 2) Use Feature: keyword to pass what "agile story" will be covered in the feature file.
 3) Write Scenario:
 4) Add/create steps to this scenario using Given, When, Then, And, But keywords.
 5) We run the scenario from RUNNER CLASS to get snippets(unimplemented methods) to implement.
 6) Copy and paste snippets into step definition class that is related to that feature.
 7) Implement java+selenium+junit... programming logic to actually automate each step

# TestNG vs JUnit ? 
- in Cucumber, we implement the scenario outline in feature files. However, I can write the java code here.
- 

    

