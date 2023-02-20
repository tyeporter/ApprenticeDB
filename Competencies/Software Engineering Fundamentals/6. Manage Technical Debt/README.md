# Understand and manage technical debt

### Understand the issues caused by technical debt

This also answers:
- "Demonstrate ability to identify technical debt"
- "Demonstrate ability to eliminate technical debt"

[🎗️ Technical Debt](/Certificates/Technical%20Debt%20Certificate.pdf)

Technical debt can be metaphorically understood through financial debt. We usually take on financial debt to purchase something that we wouldn't have been able to if we didn't borrow the money. A similar thing happens with technical debt. We usually deliberately take on some form of technical debt so that we can release to market faster. Just as we may get into so much financial debt we are unable to pay it, we could get into so much technical debt that it's almost impossible to maintain. Technical debt may take many shapes. Along with code debt there's also debt within documentation, architectural debt, dependency debt, test debt and even knowledge debt. An example of documentation debt would be having design and/or specification docs in the database which are outdated and not maintained. As the product grows and adds more features, more and more docs are being piled into the database, making it difficult for employees to find accurate information. An example of code debt would be tightly couple code. Tightly coupled code can make it hard to understand and update our code. As we continue to use a tightly coupled architecture, these issues become even worse and a single bug may break our entire product. Since our code isn't modular/flexible, it's difficult to test each component. We could avoid tight coupling by using good coding standards like SOLID and CLEAN CODE principles (created by Robert C. Martin). If we already have technical debt that we want to tackle, we first need to convince our team why we should deal with existing technical debt. If there is tangible evidence that the technical debt is causing significant customer/revenue loss for example, then our team would likely support this effort. Next, we would have to create a game plan for "paying off" this technical debt. This can be based on short-term/long-term/quarterly goals and developers can report on progress over the lifetime of the project. Finally, the team should come up with some architectural guidelines that developers can follow. Peer programming and code review can help with assuring developers are understanding and following team coding standards.



### Understand ability to use code scanning and static analysis tools

Using SonarQube to scan [🏗 StorefrontAPI](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI) project for vulnerabilities and technical debt:

![](/Images/sonar_debt.png)
![](/Images/sonar_pass.png)