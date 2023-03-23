# Understand and manage technical debt

## Table of Contents
- [Explanation](#explanation)
- [Example](#example)
- [Certificates](#certificates)

### Explanation

Technical debt can be metaphorically understood through financial debt. We usually take on financial debt to purchase something that we wouldn't have been able to if we didn't borrow the money. A similar thing happens with technical debt. We usually deliberately take on some form of technical debt so that we can release to market faster. Just as we may get into so much financial debt we are unable to pay it, we could get into so much technical debt that it's almost impossible to maintain. 

Technical debt may take many shapes:
- Code Debt 
- Documentation Debt
- Architectural Debt
- Dependency Debt
- Test Debt 
- Knowledge Debt
- etc. 

An example of documentation debt would be having design and/or specification docs in the database which are outdated and not maintained. As the product grows and adds more features, more and more docs are being piled into the database, making it difficult for employees to find accurate information. An example of code debt would be tightly couple code. Tightly coupled code can make it hard to understand and update our code. As we continue to use a tightly coupled architecture, these issues become even worse and a single bug may break our entire product. Since our code isn't modular/flexible, it's difficult to test each component. 

#### **EXPECTATIONS & OUTCOME**

The effort of removing technical debt will have many benefits which includes:
- Get rid of "code smell" by using DRY and SOLID principles
- Code becomes more maintainable and less of a hinderance for developers
- Less of a security risk when getting rid of dependency debt
- Less time and money will be spend fixing / patching bugs 
- Less time spent going through documentation that's obsolete
- Ability to keep up with industry practices and standards
- Ability for teams to act and iterate quickly

### Example

**Real-World Example**: Technical Debt within CoreToolKit as discussed in the automation presentation

**Visualizing Technical Debt**: 

In the example below, I'm doing a quality check for the [🏗 StorefrontAPI](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI) project I worked on in [Full Stack JavaScript](/Certificates/Full%20Stack%20JavaScript%20Developer%20Certificate.pdf). As you can see, the project passes quality standards, but still has some technical debt that I could get rid of such as:
- Getting rid of *duplicate* methods
- Getting rid of *deprecated* methods

This has allowed me to see that although I'm using Clean Code principles, I could improve the code quality by incorporating DRY and SOLID as well.

| [🏗 StorefrontAPI](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI) Quality Check w/ SonarQube |
| ---- |  
| ![](/Images/sonar_debt.png) |
| ![](/Images/sonar_pass.png) |


### Certificates

- [🎗️ Technical Debt Certification](/Certificates/Technical%20Debt%20Certificate.pdf) (Video Based)
    - Includes coding examples
