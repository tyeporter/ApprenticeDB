# Understand and demonstrate how to build and test quality code, at scale

## Table of Contents
- [Demonstration](#demonstration)
- [Certificates](#certificates)

### Demonstration

The only project I worked on during my learning that involved building and testing quality code at scale was for the [🏗 Udagram](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/nd0067-c4-deployment-process-project-starter) project in Udacity's [Full Stack JavaScript program](https://www.udacity.com/course/full-stack-javascript-developer-nanodegree--nd0067). This project was assigned for the 4th (and last) module of the course: **"Deployment Process"**. The goal for the project was to take a Full Stack application, configure a CI / CD pipeline for the project to be built, tested and deployed from, and configure set of AWS services that will host the application.

#### **OBJECTIVES & OUTCOMES**

The reason for building the project was to demonstrate that I had gained the necessary knowledge to build, test, and deploy a fullstack application at using a CI / CD pipeline. Topics covered in this module included:
- Tools and Environments needed for the deployment process
- Building a production-ready development environment
- Creating users using AWS IAM (Identity and Access Management)
- Creating databases with AWS RDS (Relational Database Service)
- Creating a web app environment instance with Elastic Beanstalk
- Creating "Buckets" using AWS S3 (Simple Storage Service)
- Deploying to S3 using AWS CLI
- Deploying to Elastic Beanstalk using EB CLI

After the training, I was able to:
- Configure CI/CD pipeline using Github, CircleCI and AWS
- Configure job that requires manual deployment using CircleCI
- Configure a PostgreSQL database with required specs using AWS RDS
- Configure a Node.js environment for the backend application using Elastic Beanstalk
- Configure a "bucket" of resources available to the public using AWS S3 so that users can access the frontend application 
- Configure CircleCI "Orb" for setting up server to download necessary tools (Node.js, AWS CLI, EB CLI, etc.) and secrets so that it can build, test, and deploy apps to configured AWS environments 

#### **PROJECT REQUIREMENTS**
As per the requirements, the application and pipeline needed to have the following functionality:
- Application
    - Allow user to register using name, email, and password
    - Encrypt user password using bcrypt and persist details in a PostgreSQL database
    - Allows users to sign in using email and password 
    - Authorize profile access and manage session using JWTs
    - Allow signed up users to upload photos to their profile
    - Allow users to view a feed of uploaded photos
- Pipeline
    - Ability to install dependencies needed to run and test the front and backend applications using CircleCI
    - Ability to run tests for both applications using CircleCI
    - Ability to build a production version of the applications using CircleCI
    - Ability to manually deploy the production builds of the applications to AWS using CircleCI
    - Ability to host the production builds of the applications using AWS

#### **PIPELINE ARCHITECTURE**
You can find diagrams of the architecture I used in the projects [screenshots]() directory, but I will describe and show here as well.

- Continuous Integration and Development
    - Github (Code Repository)
    - Github Actions (Initiate CI / CD Process; Pushing Updates CircleCI)
    - CircleCI (For Building, Testing, and Deploy)

    <br>

    ![](/Images/pipeline_diagram.png)
    
- Hosting
    - AWS S3 (For Hosting Frontend)
    - Elastic Beanstalk (For Hosting Backend)
    - AWS RDS (For Hosting Database)

    <br>

    ![](/Images/infrastructure_diagram.jpg)
![](https://github.com/4orter/Learning/blob/main/Udacity/Fullstack%20JavaScript%20Nanodegree/nd0067-c4-deployment-process-project-starter/screenshots/pipeline_diagram.png)


### Certificates
- [🎗️ Full Stack JavaScript Developer Certificate](/Certificates/Full%20Stack%20JavaScript%20Developer%20Certificate.pdf) (Merit Based)
    - Includes videos, quizzes and graded projects
- [🎗️ Test-Driven Development Certificate](/Certificates/Test-Driven%20Development%20Certificate.pdf) (Concept / Video Based)
    - Includes coding examples
- [🎗️ Clean Code Certificate](/Certificates/Clean%20Code%20Certificate.pdf) (Concept / Video Based)
    - Includes coding examples
- [🎗️ Building Development Environments](/Certificates/Development%20Environment%20Certificate.pdf) (Concept / Video Based)
    - Includes coding examples
- [🎗️ Github Certificate](/Certificates/Github%20Certificate.pdf)  (Concept / Video Based)
    - Includes examples
- [🎗️ Continuous Integration and Development Certificate](/Certificates/CICD%20Certificate.pdf) (Concept / Video Based)
    - Includes examples
- [🎗️ Jenkins Certificate](/Certificates/Jenkins%20Certificate.pdf) (Concept / Video Based)
    - Includes  examples
