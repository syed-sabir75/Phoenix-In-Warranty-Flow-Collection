# Postman API Automation integration with Github Actions #

This repository is a demonstration for POC for integrting postman tests with github action. The test are written in postman and they are executed on the VM with the help of newman and
newman-reporter-htmlextra.Github Actions will trigger the project execution on every push to the main branch. You can also executed the project manually using workflow_dispatch. The Project runs
on a scheduled time with the help of the cron job.

The HTML report is archieved and kept in the artifact section for the team to download it. Along with that they can view the report directly from the github page : https://syed-sabir75.github.io/Phoenix-In-Warranty-Flow-Collection/
The latest report is mailed to the team members using Gmail SMTP.

## About Me ##
Hi My Name is Syed Sabir. I have 11 year of experience in automation Testing and DevOps. My Skillset Includes UI Automation with Selenium Webdriver, Cypress, playwright and for API Testing
I use Rest Assured and you can connect with me over: ![Linked In](https://www.linkedin.com/feed/)

## Testing Coverage ##
1. Happy Flow Testing
2. Neagtive Testing and Edge Case Testing
3. Token Testing
4. Data Driven Testing with CSV
5. Schema Validation
6. Secrets Mangement with Github Secrets 

## Tech Stack ##
1. Postman
2. Nodejs 22
3. Newman
4. Newman-Reporter-Htmlextra
5. Github Action
6. Gmail SMTP
7. Github Pages
8. CSV for Data Driven Testing
9. AWS-EC2 instance for self hosted github runner/

## Github pages ##
You can directly view the latet test report of the Postman Test at the Github Pages Link:https://syed-sabir75.github.io/Phoenix-In-Warranty-Flow-Collection/ 

## HTML Report ##
The report will be created in the newman folder 
![Postman Report](https://github.com/syed-sabir75/Phoenix-In-Warranty-Flow-Collection/blob/Static-content/Newman%20Report.png)

## Project Structure ##
```
Phoenix In-Warranty Flow Collection
├─ In-Warranty Flow Collection.postman_collection.json # Collection File 
├─ QA.postman_environment.json # Enviroment File
└─ Testdata.CSV # Testdate File

```

## How to run the project? ##
1. You can run the project on your local system for that:https://github.com/syed-sabir75/Phoenix-In-Warranty-Flow-Collection.git
2. Install Nodejs and NPM from``` http://nodejs.org/en```
3. Install Newman using ```npm install -g newman```
4. Install Newman-reporter-htmlextra ```npm install -g newman-reporter-htmlextra```
5. Run the Newman Command:
   
               ```newman run 'In-Warranty Flow Collection.postman_collection.json' \
              -e QA.postman_environment.json \
              -r cli,htmlextra \
              --reporter-htmlextra-export ./newman/index.html```

  


