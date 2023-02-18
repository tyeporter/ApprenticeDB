# Understand and demonstrate how to build and test quality code, at scale

### Understand how to build quality code at scale

Building quality code at scale involves adhering to good software engineering practices like Agile development, Scrum, SOLID principles and Clean Architecture. It also involves using modern practices like Continuous Development and Continuous Integration and making sure that code is being tested at every step of the Software Development Lifecycle.

Testing and CI/CD demonstration:

![](/Images/circleci_1.png)
![](/Images/circleci_2.png)

### Understand the techniques used for ensuring quality

[🎗️ Certificate](/Certificates/Test-Driven%20Development%20Certificate.pdf)
- **"Test-Driven Development in Action"** Section
- **"Strategies and Techniques for Testing Code"** Section
- **"Looking out for Test-Driven Development Gotchas"** Section

### Understand the different types of testing, where to apply them, and the relative amounts

[🎗️ Certificate](/Certificates/Test-Driven%20Development%20Certificate.pdf)

- **"Different Ways of Testing Application"** Section

### Understand the successful use of test coverage tools

The successful use of test coverage tools involves using coverage metrics to make informed decisions on how we can improve the *quality* of our tests and essentially increase the percentage of code covered by tests.

Code coverage tool demonstration:

![](/Images/code_coverage.png)

### Understand successful use of performance testing

The successful use of performance testing involves using performance metrics to make decisions on how to improve the *performance* of our application/services. Performance testing tools like Artillery and JMeter will simulate sending several requests (load) to our API which will help us test how our service performs under different stressors. This allows us to uncover issues like poor performing code, memory leaks, long response times, etc. It will also give us insights into how we may want to scale our application. Maybe under certain stress we would want to horizontally scale (our application) versus vertically scale (our resources), or vice-versa.

### Understand successful use of boundary and limit testing

The successful use a boundary testing involves using ranges (or partitions) to test the limits of functionality within our application, given that our code is modular and testable. For example, we may have a request service in our application that allows users of different tiers to make requests within a certain range:
- Starter Tier  
    - 1 - 500 req. / month
- Regular Tier
    - 1 - 10000 req. / month
- Enterprise Tier
    - 1 - 1000000 req. / month

When it comes to our request service, the above partitions are *valid*. For example, the amount of requests serviced for a Starter Tier user should fall within the range of 1 - 500. Anything falling outside of this range would be *invalid* and therefore would fail the boundary test.

### Understand successful use of chaotic testing

The successful use fo chaotic testing involves using tools like Gremlin and Load Impact to improve the *resiliency* of our software infrastructure. For example, our application should be able to replicate itself if it's under heavy load or one of its instances is terminated. If an AWS availability zone shuts down, AWS should have the infrastructure in place to recover that zone, and we should still be able to service customers while the zone is down. If one of our databases becomes corrupted, we should have replicas in place that will replace it. By exposing the weak points of our infrastructure, chaotic testing helps improve our service's reliability and availability. Therefore, increasing the confidence that users have in our product.
