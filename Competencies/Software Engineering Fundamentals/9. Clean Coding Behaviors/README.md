# Understand, articulate, and demonstrate clean coding behaviors

### Demonstrate use of refactoring to yield clean code 

This also answers:
- "Demonstrate ability to write code with clarity"
- "Demonstrate ability to write code that minimizes duplication"
- "Demonstrate ability to write code with simplicity"
- "Demonstrate use of SOLID principles in code"

Certificate: [🎗️ Clean Code Certificate](/Certificates/Clean%20Code%20Certificate.pdf)

I use clean code and SOLID principles in many of many example projects including: [🏗 ImageProcessingAPI](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/ImageProcessingAPI), [🏗 Casts](https://github.com/4orter/Learning/tree/main/WozU-SDET/projects/Casts), [🏗 OnTheMap](https://github.com/4orter/Learning/tree/main/Udacity/iOS%20Nanodegree/OnTheMap), [🏗 StorefrontAPI](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI) and more.

- Single Responsibility Principle
    - **Example**: The [image manipulation](https://github.com/4orter/Learning/blob/main/Udacity/Fullstack%20JavaScript%20Nanodegree/ImageProcessingAPI/src/util/image-manipulation.util.ts) utility module in [🏗 ImageProcessingAPI](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/ImageProcessingAPI) focuses specifically on manipulating images using the [Sharp](https://github.com/lovell/sharp) library. It doesn't deviate from its specific role.
- Open-Closed Principle
    - **Example**: The [withHover](https://github.com/4orter/Learning/blob/main/ui.dev/github-battle-vercel/app/components/withHover.jsx) higher-order component in [🏗 github-battle-vercel](https://github.com/4orter/Learning/tree/main/ui.dev/github-battle-vercel) embraces this principle. Instead of modifying classes directly, we create a higher-order component that will allow us to extend the functionality of our class component.
- Liskov Substitution Principle
    - **Example**: When calling the `render()` method on any class that inherits from `React.Component`, it will always return a JSX element or an object describing the DOM element.
- Interface Segregation Principle
    - **Example**: The [BusinessUsable]() interface in [🏗 StorefrontAPI](https://github.com/4orter/Learning/tree/main/Udacity/Fullstack%20JavaScript%20Nanodegree/StorefrontAPI) is used specifically for business processes.
- Dependency Inversion Principle
    - **Example**: Protocols in iOS development are used to decouple view controllers from one another. In [LoginViewController](https://github.com/4orter/Learning/blob/caea66475e5f3db60f2470dcc2b844c78ce42c62/Udacity/iOS%20Nanodegree/OnTheMap/OnTheMap/Controller/Login%20View%20Controller/LoginViewController.swift) of [🏗 OnTheMap](https://github.com/4orter/Learning/tree/caea66475e5f3db60f2470dcc2b844c78ce42c62/Udacity/iOS%20Nanodegree/OnTheMap) we create a protocol, `LoginViewControllerDelegate`, that allows us to delegate tasks to any other view controller that implements the protocol (also known as "interface" in other languages).

### Explain the various clean coding principles represented by the acronym SOLID

I answered this previously in [1. Key Computing Fundamentals](https://github.com/4orter/ApprenticeDB/tree/main/Competencies/Software%20Engineering%20Fundamentals/1.%20Key%20Computing%20Fundamentals)



