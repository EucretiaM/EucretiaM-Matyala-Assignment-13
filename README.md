Assignment 13 reflects on setting up a CI/CD pipeline using GitHub Actions to automate testing, enforce branch protection
rules, and generate release artifacts.

A CI/CD pipeline in GitHub automates the software development lifecycle, specifically the build, test, and deployment stages. 
It uses tools like GitHub Actions to streamline the process of integrating code changes, verifying them, and delivering the application to production. 

THE BREAKDOWN OF CI/CD:

CONTINUOUS INTERGRATION (CI):
This phase involves automatically integrating code changes from developers into a shared repository. It includes tasks like building, testing, and merging new code. 

CONTINUOUS DELIVERY/DEPLOYMENT (CD):
CD automates the next stages, including deploying the built code to different environments (staging, production). 
Continuous deployment goes a step further, automating the deployment to production without human intervention. 
GitHub Actions:
This is a platform within GitHub that allows users to create custom workflows for their CI/CD pipelines. 
It can be used to automate tasks like packaging, releasing, and deploying applications

By automating these processes, CI/CD pipelines help: 

Speed up the development process:
Automated testing and deployment reduce manual efforts and release cycles.

Improve code quality:
Automated tests help identify and fix errors early in the development process.

Reduce deployment risks:
Automated deployments are more reliable and less prone to errors than manual deployments.

Enable faster releases:
Automated pipelines allow for more frequent releases of new features and bug fixes.

HOW TO RUN TESTS LOCALLY

Use npm or yarn to install your chosen framework as a dev dependency. For example, using Mocha

Code:
npm install --save-dev mocha

  // test/example.test.js
    const assert = require('assert');
    const { myFunction } = require('../myModule');

    describe('My Function', () => {
        it('should return the correct value', () => {
            assert.strictEqual(myFunction(2), 4);
        });
    });

.

PR BLOCKED FAILURES TESTS

![image](https://github.com/user-attachments/assets/b46a4ab6-169a-45dc-a201-aef7465b6ff5)

![image](https://github.com/user-attachments/assets/d7cbe932-6ad1-48a8-ba96-84f7ba3d9836)


