# Understand and demonstrate test-driven development

## Table of Contents
- [Explanation](#explanation)
- [Example](#example)
- [Certificates](#certificates)

### Explanation

There are 3 main types of test-driven development are:
- Plain Test-Driven Development
    - In plain TDD, the code that we right is determined by our test cases. This is usually referred to as the *Red, Green, Refactor* methodology. First, we write our test case  which will initially fail (Red). Then, we write functional code to make the test pass (Green). Last, we organize (or Refactor) our code using software architecture, data structures, SOLID principles, etc.
    
- Behavioral-Driven Development
    - In BDD, the code that we write is determined by user requirements and system behavior. This is usually referred to as the *Given-When-Then* method which helps describe requirements in simple language format like Gherkin. For example, "**given** a user is logged into their account", "**when** the user clicks on the the settings icon", "**then** display a page with user's account information".
    
- Acceptance Test-Driven Development
    - In ATDD, the code that we write is determined by user requirements, similar to BDD. This method focuses more on acceptance criteria and requires collaboration between developers, testers, and users. In ATDD, we typically try to answer 3 questions: "What are we trying to solve?", "How can we solve it?", "Can we solve it this way?" Just like in BDD, acceptance tests would be written in a simple language format like Gherkin.
   

#### **EXPECTATIONS & OUTCOMES**
- For plain test-driven development, we are able to: 
    - Clarify requirements before development
    - Have a fast feedback loop
    - Have less chance of code breaking down the line since we're constantly testing
    - Have developers be more confident when creating new features
    
- For behavior driven development, we are able to:
    - Make it easy for developers to understand requirements before writing tests
    - Focus on system behavior which can cut development costs since we're not spending time writing unnecessary tests
    - Help non technical employees better to understand test requirements 
    - Illustrate real-world user behavior using scenarios
  
 - For acceptance test driven development, we are able to:
    - Clarify system requirements at multiple levels, reducing the amount of cross-team friction
    - Focus on real-world use, which can cut development costs similar to BDD since we're not spending time writing unnecessary tests
    - Foster cross-team and user collaboration which can lead to a better product for the user

### Example

In the following [🏗 Add to Cart](https://github.com/4orter/Learning/tree/main/YourLearning/Selenium/Selenium%20Webdriver%20with%20TypeScript/SeleniumTS/tests/cucumber) example, I use behavior driven development with the Cucumber framework to confirm that requirements of the `add-to-cart` functionality of the website are being met. In order for the test to pass, a modal should be visible after click the `add-to-cart` button at the specified URL.
 
|[🏗 Add to Cart](https://github.com/4orter/Learning/tree/main/YourLearning/Selenium/Selenium%20Webdriver%20with%20TypeScript/SeleniumTS/tests/cucumber) BDD Example w/ Cucumber |
| ---- |
| ![](/Images/bdd_cucumber.png) | 

As you can see on the left, we define system behavior in a `.feature` file using the *Given-When-Then* pattern. Each feature file should have an equivalent "Steps" file that is responsible for implementing the test (on the right). Each part of the *Given-When-Then* pattern has its own method which is responsible for taking some action or asserting some information:
- In the case of *Given*
    - Its method is responsible for setting up initial state. In this specific example, navigating to the correct webpage. 
- In the case of *When*
    - Its method is responsible for taking some action. In this example, clicking on the `add-to-cart` button.
- In the case of *Then* 
    - Its method is responsible for asserting an outcome or some information. In this case, that the modal is showing.


### Certificates

- [🎗️ Test-Driven Development Certification](/Certificates/Test-Driven%20Development%20Certificate.pdf) (Video Based)
    - Included code examples
- [🎗️ Node.js Unit Testing Certificate](/Certificates/Node.js%20Unit%20Testing%20Certificate.pdf)(Video Based)
    - Included code examples
- [🎗️ Python Unit Testing Certificate](/Certificates/Python%20Unit%20Testing%20Certificate.pdf)(Video Based)
    - Included code examples
- [🎗️ React Testing Certificate](/Certificates/React%20Testing%20Certificate.pdf) (Text Based)
    - Include code exercises and quizzes