[home](../README.md)
# [Development Practices](README.md) - Code Quality


There are many features that make up a code's quality:

* **Readability**: Can the code be easily read by others? If so, then it would be much easier for others to maintain
* **Documented/Commented**: Ideally, code should be self-explanatory but it is recommended comments to explain the workings to future developers
* **Future Proof**: Whilst it isn't feasible to know all the changes that would be required down the line, code should be written so that it can be easily extended without major refactoring
* **Efficiency**: Code that can perform its function more efficiently
* **Testability**: Having suites of automated tests enables the team to make changes with increased confidence that their changes will not adversely effect the current functionality


Regular code reviews and Paired Programming (AKA. Extreme Programming) are good approaches to maintain high levels of code quality.

There are many tools available to automatically rate code quality (e.g. SonarQube, Veracode, Deepscan). These tools should be added to the build pipeline so that they fail the build if the quality of the code falls below the agreed threshold (e.g. all new code must have > 80% unit test coverage). See [quality gate enforcement](../continuous-delivery/quality-gate-enforcement.md).

Many IDEs have plugins to identify issues before they are pushed to the repository. This approach of "Shifting Left" helps to catch and fix issues as early as possible.


**Further reading**:
* [Google Style Guides](https://google.github.io/styleguide/)
* [Coding Standards and Best Practices to Follow](https://www.browserstack.com/guide/coding-standards-best-practices)