# *How release happens ?*
- Every 2 weeks we release new version.
- Release is happening manually. 
- We click release manually. Everything else is automated Smoke, regression, performance are done automatically. At the end on Saturday morning at 10 am we release new version. 

# What tools do you use for CI/CD ? 
- We use Jenkins. 
    
- **benefits:**
    - open source (free)
    - lots of plugins
    - big community ( easy to troubleshoot )
  

      other tools: CircleCI, GitLab, TeamCity, Bamboo, GitHub actions, etc.


# What are the disadvantages of Jenkins ?
- slow , no good support because it's free tool, you have to provision and manage server with a Jenkins yourself. Difficult to write pipeline script comparing to other solutions.

# Difference between freestyle project and pipeline script in Jenkins ?
- Freestyle project is used to create the most basic Jenkins job.
- Jenkins job - task for Jenkins to automate something. 
- Pipeline script - it's a more advanced way to create a jenkins job. Jenkins started supporting pipeline scripts from version 2 (whereas freestyle project was introduced in the very first version). 
- If in case of freestyle project you have select steps from drop-downs, pipeline gives you a lot of freedom with groovy script. You can create if statements, setup parallel jobs, put try/catch blocks etc..
- Groovy script - language that is used to write Jenkins pipelines. Based on Java.