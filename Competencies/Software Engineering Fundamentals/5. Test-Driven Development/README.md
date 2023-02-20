# Understand and demonstrate test-driven development

### Articulate the differences and relative strengths / weakness of the various models of test-driven or behavior driven development

I'm assuming this is talking about the different types of test-driven development. If this is the case, there are 3 main types:
- Test-Driven Development
    - In regular TDD, the code that we right is determined by our test cases. This is usually referred to as the *Red, Green, Refactor* methodology. First, we write our test case  which will initially fail (Red). Then, we write functional code to make the test pass (Green). Last, we organize (or Refactor) our code using software architecture, data structures, SOLID principles, etc.
    - **Pros**: 
        - Clarifies requirements before development
        - Fast test feedback loop
        - Less chance of code breaking down the line
        - Higher developer confidence when creating new features
    - **Cons**:
        - Slows down development time
        - Easy for developers to bypass when needing to add new features
        - Can feel tedious for developers who haven't used this method before
- Behavioral-Driven Development
    - In BDD, the code that we write is determined by user requirements and system behavior. This is usually referred to as the *Given-When-Then* method which helps describe requirements in simple language format like Gherkin. For example, "**given** a user is logged into their account", "**when** the user clicks on the the settings icon", "**then** display a page with user's account information".
    - **Pro**:
        - Easy for developers to understand requirements
        - Focused on system behavior which can cut development costs
        - Better to understand for non technical employees
        - Illustrates real-world user behavior
    - **Cons**:
        - Slow development time when creating scenarios
        - Slows test creation time when translating statements into code
        - More files to be maintained
- Acceptance Test-Driven Development
    - In ATDD, the code that we write is determined by user requirements, similar to BDD. This method focuses more on acceptance criteria and requires collaboration between developers, testers, and users. In ATDD, we typically try to answer 3 questions: "What are we trying to solve?", "How can we solve it?", "Can we solve it this way?" Just like in BDD, acceptance tests would be written in a simple language format like Gherkin.
    - **Pros**:
        - System requirements are clarified at multiple levels
        - Focuses on real-world use, which can cut development costs
        - Fosters cross-team and user collaboration
    - **Cons**:
        - Collaboration for writing acceptance tests slows down development
        - More documents to maintain for a single test
        - ATDD tools may end up being too technical for non-technical collaborators


### Demonstrate use of various models of test-driven or behavior driven development

Using Cucumber with TypeScript and Gherkin to verify the behavior of a website:

![](/Images/bdd_cucumber.png)