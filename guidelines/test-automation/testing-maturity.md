[home](../README.md)
# [Test Automation](README.md) - Testing Maturity


**Common Pitfalls regarding Test Automation**

* Not having developers involved in testing. DORA’s research shows that when developers are primarily responsible for creating and maintaining suites of automated tests, and when it is easy for developers to fix acceptance test failures, this drives improved performance. When other groups own the test automation, two problems often arise:
    * **Test suites are frequently in a broken state**. Code changes might require tests to be updated. If developers are not responsible for test automation, the build pipeline stays broken until the responsible team fixes the tests.
    * **Developers write code that is hard to test**. Developers tend to solve the problem they are given without thinking about how it will be tested. This can lead to poorly designed code and expensive, hard-to-maintain test suites.
* Failing to curate your test suites. Make sure you continuously review and improve your test suites to better find defects and keep complexity and cost under control. For example:
    * Acceptance test suites should typically represent real [end-to-end](https://testing.googleblog.com/2016/09/testing-on-toilet-what-makes-good-end.html) user journeys through the system, rather than just collections of automated acceptance criteria. As your product evolves, so will these scenarios, and the test suites validating them. For more information on this process, see the video [Setting a Foundation For Successful Test Automation by Angie Jones](https://www.youtube.com/watch?v=qYfI2-bC6LA).
    * If every time you change your code you must also change multiple unit tests, you’re probably [over-relying on mocking](https://martinfowler.com/articles/mocksArentStubs.html), or failing to prune your unit test suite.
    * Keep your test suites well-factored. If every change to your UI causes multiple acceptance tests to fail, use the [page object pattern](https://martinfowler.com/bliki/PageObject.html) to decouple your tests from the system under test.
    * If your tests are expensive to maintain, this could point to problems with your software’s [architecture](https://dora.dev/devops-capabilities/technical/loosely-coupled-architecture). Make sure you continue to invest in making your software easy to test, including incorporating [refactoring](https://refactoring.com/) into your team’s daily work.
* Having the wrong proportion of unit and acceptance tests. A specific design goal of an automated test suite is to find errors as early as possible. This is why faster-running unit tests run before slower-running acceptance tests, and both are run before any manual testing.
* You should find errors with the fastest category of test. When you find an error in an acceptance test or during exploratory testing, add a unit test to make sure this error is caught faster, earlier, and cheaper next time. Mike Cohn described the ideal [test automation pyramid](https://books.google.com.br/books?id=8IglA6i_JwAC&printsec=frontcover&dq=Mike+Cohn+Succeeding+with+Agile&hl=pt-BR&sa=X&ved=0ahUKEwj9x8S8tuTiAhWjGLkGHU0GCxEQ6AEILTAA#v=onepage&q=Mike%20Cohn%20Succeeding%20with%20Agile&f=false), shown in the following diagram, where most of the errors are caught using unit testing.

![Test Pyramid](../../images/testing-maturity-pyramid.png)

Tolerating unreliable tests. Tests should be reliable: that is, when the tests pass we should be confident the software is releasable, and test failures should indicate a real defect. In particular, don’t tolerate flaky tests


---
**Further reading**:
* [Google’s mitigation strategy for flaky tests](https://testing.googleblog.com/2016/05/flaky-tests-at-google-and-how-we.html).
