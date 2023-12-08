[home](../README.md)
# Continous Delivery


## [Source Control](source-control.md)
Source control enables teams to manage and track changes to their codebase efficiently, reducing the risk of conflicts and enabling parallel development. It provides a structured approach to versioning and collaboration, allowing teams to work seamlessly across different branches and environments. It enhances transparency, accountability, and traceability in the development process, facilitating quicker error detection and resolution. By fostering collaboration, reducing rework, and improving code quality, source control plays a pivotal role in expediting software development workflows and ensuring the swift delivery of high-quality products.


## [Build Reliability](build-reliability.md)
Broken or failing builds in a CI/CD pipeline can deteriorate a team's faith in its own processes. It can also hinder a team's ability to efficiently deliver high-quality software. That's why it's important to identify and fix broken builds in a CI/CD pipeline. Best practices for identifying broken builds include: Make sure it builds locally, ensure sufficient logging on the build server, have a way of inspecting the file system and implement alerts.


## [Deployment Process](deployment-process.md)
Having the right deployment process in place can help ensures that new features, updates, and fixes can be swiftly and reliably moved from development to production environments. There are two versions of deployment that are commonly encountered (Unique Version pattern, Co-existing Version pattern)


## [Configuration](configuration.md)
Configuration management helps engineering teams build robust and stable systems using tools that automatically manage and monitor updates to configuration data. Complex software systems are composed of components that differ in granularity of size and complexity. Some examples of software configuration metadata are:
* Specifications of computational hardware resource allocations for CPU, RAM, etc.
* Endpoints that specify external connections to other services, databases, or domains
* Secrets like passwords and encryption keys


## [Change Management Controls](change-management-controls.md)
The right change management control process is a crucial element in accelerating flow within an organization. It establishes a structured and controlled approach to implementing changes while minimizing disruption and risk. By providing clear guidelines and approvals for changes, it ensures that updates are thoroughly tested and documented, reducing the likelihood of errors or unexpected issues.


## [Quality Gate Enforcement](quality-gate-enforcement.md)
A quality gate is an enforced measure built into your pipeline that the software needs to meet before it can proceed to the next step. This measure enforces certain rules and best practices that the code needs to adhere to prevent poor quality from creeping into the code.

Quality gates are typically automated, allowing the pipeline to self-monitor the quality of delivered code.


## [Security & Compliance](security-and-compliance.md)
Integrating security tooling and testing in CI/CD pipelines ensures a fast feedback loop for the developer when any security vulnerabilities are detected. This is a pattern often referred to as shifting security left referring to earlier in the pipeline diagram. Adopting shift left provides the team higher confidence in delivering software free of security vulnerabilities.
