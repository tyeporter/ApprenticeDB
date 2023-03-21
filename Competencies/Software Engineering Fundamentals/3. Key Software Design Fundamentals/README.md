# Understand and demonstrate key software design fundamentals

## Table of Contents
- [Demonstration](#demonstration)
- [Certificates](#certificates)

### Demonstration

The [🏗 StorefrontAPI](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI) project is a Node.js / Express project I worked on during the apprenticeship while going through [this](https://www.udacity.com/course/full-stack-javascript-developer-nanodegree--nd0067) FullStack JavaScript Program. The requirements for the project and the rubric / grade was given by a Udacity mentor. The goal for the project was to build a storefront backend for an hypothetical storefront.

#### **PROJECT REQUIREMENTS**
As per the requirements, the backend needed to have the following functionality:
- The ability for users to sign up, sign in and sign out
- The ability for administrators to create, update and view products and categories
- User authentication and password encryption
- User authorization and session management using JWTs
- Creating endpoints for the following:
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
- Node.js (Runtime)
- TypeScript (Language)
- Express (Web Framework)
- PostgreSQL (Database)
- db-migrate (Database Migration)
- JWT and Bcrypt (Auth)
- Jasmine (E2E Testing)

#### **PROJECT SETUP**
The project's [README](https://github.com/4orter/Learning/blob/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI/README.md) goes through the steps for setup, how to run the project, functionality, and available API endpoints that you can use. Note that you need to have Node.js (v16) and PostgreSQL installed on your system to run the project.

### Certificates
- [🎗️ Full Stack JavaScript Developer Certificate](/Certificates/Full%20Stack%20JavaScript%20Developer%20Certificate.pdf)
- [🎗️ The Complete Java Development Bootcamp Certificate](/Certificates/Java%20Bootcamp%20Certificate.pdf)
- [🎗️ Core Python Certificate](/Certificates/Core%20Python%20Certificate.pdf)
- [🎗️ The Modern JavaScript Bootcamp Certificate](/Certificates/Modern%20JavaScript%20Bootcamp%20Certificate.pdf)
- [🎗️ Node.js: Getting Started Certificate](/Certificates/Node.js%20Certificate.pdf)