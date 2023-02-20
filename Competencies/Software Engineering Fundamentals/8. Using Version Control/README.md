# Understand how to use version control for all elements of the software delivery lifecycle

### Understand the principles of version control

This also answers:
- "Understand versioning, releases, issues, and merges in source code"

[🎗️ Github Certificate](/Certificates/Github%20Certificate.pdf)

Version control software like Git allow teams to track and document code over time. With Git, teams can create repositories which will house the codebase. The repository will usually have a main/master branch which serves as the source of truth for the codebase. When developers need to make updates, they typically create a separate branch from the main branch and then make their changes. Once the developer's updates are ready, they can stage and commit their changes to their separate branch. After that, the developer can make a pull request to merge the changes in their branch into the main branch. Usually, this pull request would go through thorough review and testing. If the developer's changes conflict with changes elsewhere, they may need revert changes or coordinate with other developers to resolve these conflicts. Once the pull request passes all tests and the reviewer(s) approve the request, the developer can then merge their changes into main and delete their separate branch. Github and Gitlab improves on Git by providing servers, a GUI, and many other tools that teams around the globe can use to collaborate on software projects. For example, teams can use tools like Github Actions and CI/CD tools like CircleCI to deliver new versions of software to users when a certain criteria is met in our repository. All of these things makes delivering software more secure and efficient.

The rate at which teams release software to the public depends on their decided release schedule. This could be weekly, monthly, or even quarterly/ Developers typically use semantic versioning to label the release. An example would be "`v2.3.1`", where, in this case:
- `2` represents the major version / release
    - We'd increment this number if we made breaking changes in our code
- `3` represents the minor version / release
    - We'd increment this number if we made non-breaking feature updates
- `1` represents the patch version /release
    - We'd increment this number if we are making non-breaking patch updates

Teams can use WebHooks in their CI/CD pipeline to clone, build and release software when a tag (with a new release version) is pushed to the project repository.

### Understand the use of dependencies and libraries from within and outside the team

We can use semantic versioning when we need a specific version of a library. For example, a Front-End developer may want to use the lastest version of React `18`. He / she could signify this in their `package.json` like the following:

```json
{
    "name": "RandomProject",
    ...
    "dependencies": {
        "react": "^18.0.0",
        "react-dom": "^18.0.0",
    }
}
```

In the above example, the caret symbol (`^`) signifies that we want to use the latest version of major version `18`. So, that could be `18.2.1` or `18.3.4`. It won't download anything above or below `18`.

### Demonstrate proper usage of versioning, releases, issues, and merges in source code

![](/Images/merging.png)
![](/Images/versioning.png)
> Parts redacted for privacy


### Demonstrate usage of dependencies and libraries from within and outside the team

- Used Ruby Gemspec for internal and external dependencies for MaaS360 Zscalar project
- Using NPM for external dependencies: [package.json](https://github.com/4orter/Learning/blob/main/ui.dev/github-battle-vercel/package.json)