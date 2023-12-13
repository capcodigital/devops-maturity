[home](../README.md)
# [Test Automation](README.md) - Testing Strategy


A robust testing strategy is indispensable. It acts as a cornerstone for maintaining software quality and ensuring that continuous integration and delivery (CI/CD) processes run smoothly. By offering rapid feedback, it helps detect and rectify issues early in the development pipeline, reducing the time and effort required for bug fixes. Moreover, a solid testing strategy mitigates risks associated with changes, assures the reliability of existing functionalities through regression testing, and enforces consistency in testing practices. It also promotes efficiency, provides valuable insights for continuous improvement, and contributes to compliance with regulatory standards. Ultimately, a well-implemented testing strategy instills confidence in releases, enhances customer satisfaction, and supports the program's goals of accelerated software delivery and quality assurance.

![Test Pyramid](../../images/testing-strategy-pyramid.png)

Risk based testing with a focus on shift to left for early feedback is adopted for testing. Tests for features/stories need to be automated based on priority according to the risk exposure.

Two factors are used to assess the risk exposure of a test requirement, namely:

1. Business Impact
1. Likelihood of Failure

As a result of risk-based testing, risks can be mitigated effectively, and negative business impacts can be minimized.

The automation test pyramid should be followed while writing automated tests. The pyramid says that tests on the lower levels are cheaper to write and maintain, and quicker to run. Tests on the upper levels are more expensive to write and maintain, and slower to run. The percentage of UI tests should be comparatively less than the percentage of Service Tests and the percentage of Service Tests should be comparatively less than the percentage of Unit Tests to get the best return on investment.