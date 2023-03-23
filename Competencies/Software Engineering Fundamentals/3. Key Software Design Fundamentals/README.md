# Understand and demonstrate key software design fundamentals

## Table of Contents
- [Demonstration](#demonstration)
- [Certificates](#certificates)

### Demonstration

The [🏗 StorefrontAPI](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI) project is a Node.js / Express project I worked on during the apprenticeship while going through [this](https://www.udacity.com/course/full-stack-javascript-developer-nanodegree--nd0067) FullStack JavaScript Program. This project was assigned to students for the 2nd module of the FullStack JavaScript Program: **"Creating an API with PostgreSQL and Express"**. The requirements for the project and the rubric / grade was given by a Udacity mentor. The goal for the project was to build a  backend for an hypothetical storefront using a [specific set of technologies](#project-stack).

#### **OBJECTIVES & OUTCOMES**
The reason for building the project was to exemplify that I had gained the necessary knowledge and skills to become productive enough to start working on backend applications and APIs using modern standards, protocols and technologies. Topics learned in the this module included:
- SQL Basics and Setting Up Databases
- Creating APIs with Express
- Creating an API that connects to PostgreSQL
- Handling Authentication and Authorization in a Node API

After the training, I was able to:
- Write SQL queries for CRUD operations
- Create databases, schemas, and tables
- Link tables with primary and foreign keys
- Create RESTful APIs and routes using Express
- Enable CORS using Express middleware
- Secure user passwords using Bcrypt, secrets, and SALT
- Authorize access to the API using JWTs

> **NOTE**: Prior to working on projects, students when through video / quiz-based training which included small code examples and practice problems for getting hands-on experience.

#### **PROJECT REQUIREMENTS**
As per the requirements, the backend needed to have the following functionality:
- The ability for users to sign up, sign in and sign out
- The ability for administrators to create, update and view products and categories
- User authentication and password encryption
- User authorization and session management
- Support for the following through endpoints:
    - Create (POST)
        - Products (Admin only)
        - Categories (Admin only)
        - Users
        - Orders
    - Read (GET)
        - Products
        - Categories
        - Users (Admin only)
        - Orders
    - Update (PUT)
        - Products (Admin only)
        - Categories (Admin only)
        - Users
        - Orders
    - Delete (DELETE)
        - Products (Admin only)
        - Categories (Admin only)
        - Users
        - Orders

#### **PROJECT ARCHITECTURE**
I decided to use a Clean Coding architecture for the project. When viewing the project yourself, you'll see that I divide responsibility into: 
- [entities](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/src/entities) (For defining models and interfaces)
- [databases](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/src/frameworks/databases) (For defining database configuration)
- [repositories](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/src/frameworks/repositories) (For accessing data from the database)
- [use cases](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/src/use-cases) (For defining business rules)
- [controllers](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/src/controllers) (For responding to user requests) 
- [services](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/src/controllers/services) (For defining middleware used by requests)

Each part has a clear responsibility and doesn't need to change when one of the other parts gets updated. By implementing Clean Coding principles, I was able to scale the API and add new functionality seamlessly. For example, if I wanted to swap out the [PostgreSQL](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/src/frameworks/databases/postgres) database for MongoDB, I can do that by simply adding a database module specifically for MongoDB that takes care of setup and implementation. As long as the MongoDB module implements the [`DataStorable`](https://github.com/4orter/Learning/blob/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/src/entities/protocols/DataStorable.ts) interface, we are good to go ! No headache of having to refactor tightly coupled code. All we would have to do is plug the database into the [config](https://github.com/4orter/Learning/blob/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/src/config/prodConfig.ts).

#### **PROJECT STACK**
- Node.js (Runtime) [*Intermediate*]
- TypeScript (Language) [*Intermediate*]
- Express (Web Framework) [*Intermediate*]
- PostgreSQL (Database) [*Beginner*]
- db-migrate (Database Migration) [*Beginner*]
- JWT and Bcrypt (Auth) [*Beginner*]
- Jasmine (Unit / Endpoint Testing) [*Intermediate*]

#### **PROJECT SETUP**
The project's [README](https://github.com/4orter/Learning/blob/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/README.md) goes through the steps for setup, how to run the project, functionality, and available API endpoints that you can use. Note that you need to have Node.js (v16) and PostgreSQL installed on your system to run the project.


### Certificates
- [🎗️ Full Stack JavaScript Developer Certificate](/Certificates/Full%20Stack%20JavaScript%20Developer%20Certificate.pdf) (Merit Based)
    - Includes videos, quizzes and graded projects
- [🎗️ The Complete Java Development Bootcamp Certificate](/Certificates/Java%20Bootcamp%20Certificate.pdf) (Merit Based)
    - Includes videos, quizzes and workbooks
- [🎗️ Core Python Certificate](/Certificates/Core%20Python%20Certificate.pdf) (Concept / Video Based)
    - Includes coding examples
- [🎗️ The Modern JavaScript Bootcamp Certificate](/Certificates/Modern%20JavaScript%20Bootcamp%20Certificate.pdf) (Concept / Video Based)
    - Includes coding examples
- [🎗️ Node.js: Getting Started Certificate](/Certificates/Node.js%20Certificate.pdf) (Concept / Video Based)
    -  Includes coding examples