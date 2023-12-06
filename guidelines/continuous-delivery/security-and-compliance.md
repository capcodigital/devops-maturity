[home](../README.md)
# [Continous Delivery](README.md) - Security & Compliance

**Shift left**

In traditional software development you have the following 4 stages: design, develop, test and deploy. Which means testing typically happens after the development has been completed which therefore means that team will only discover significant flaws late in the process often architectural flaws late in the process which at that stage is expensive to fix. 

Shift left is the practice intended to find and prevent defects early in the software delivery process. The idea is to improve quality by moving tasks more to the left (earlier in the process) as possible.

How to implement:

**Develop security approved tools**

Providing developers with preapproved libraries and tools with input of InfoSec can help standardise the development practices within the organisation. Using tools like e.g. NexusIQ allows the organisation to flag libraries that have vulnerabilities or prevent a developer from accidentally introducing breaches within code.

**Implement quality and security scanning**

Adding quality scanning and static application security testing (SAST) as part of the CI process allows developers to get quick feedback upon checking of their code to notice if newly introduced changes are up to standard. On top of this the organisation can enforce quality standards that every product needs to adhere to.

**Develop an automated testing suite**

Creating a framework/tool for developers to be able to run end to end tests whilst they are developing before pushing code. The best way of doing this is providing developers the capability to be able to spin up the application locally or in a small virtual environment. For example creating a docker compose stack of the applications allows developers and testers to pick and choose the versions of the entire product. They can then build a new version locally subsequently adjust the docker compose configuration and run the e2e testing suite against it. This allows the developer and tester to work hand in hand and produce a higher quality of code which will have a better success rate when deploying it to live environments.
