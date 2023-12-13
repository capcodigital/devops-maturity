[home](../README.md)
# [Continous Delivery](README.md) - Change Management Controls

Two important goals of the change approval process are decreasing the risk of making changes, and satisfying regulatory requirements. One common regulatory requirement is segregation of duties, which states that changes must be approved by someone other than the author, thus ensuring that no individual has end-to-end control over a process.


**Common pitfalls in change approval processes**

The following pitfalls are common to change approval processes:

* Reliance on a centralized Change Approval Board (CAB) to catch errors and approve changes. This approach can introduce delay and often error. CABs are good at broadcasting change, but people that far removed from the change might not understand the implications of those changes.
* Treating all changes equally. When all changes are subject to the same approval process, change review is inefficient, and people are unable to devote time and attention to those that require true concentration because of differences in risk profile or timing.
* Failing to apply continuous improvement. As with all processes, key performance metrics such as lead time and change fail rate should be targeted with the goal of improving the performance of the change management process, including providing teams with tools and training to help them navigate it more effectively.
* Responding to problems by adding more process. Often organizations use additional process and more heavyweight approvals when faced with stability problems in production. Analysis suggests this approach will make things worse because this drives up lead times and batch sizes, creating a vicious cycle. Instead, invest in making it quicker and safer to make changes.


To improve your change management processes, focus on implementing the following:

* Move to a peer-review based process for individual changes, enforced at code check-in time, and supported by automated tests.
* Find ways to discover problems such as regressions, performance problems, and security issues in an automated fashion as soon as possible after changes are committed.
* Perform ongoing analysis to detect and flag high risk changes early on so that they can be subjected to additional scrutiny.
* Look at the change management process end-to-end, identifying bottlenecks, and experimenting with ways to shift validations into the development platform.
* Implement information security controls at the platform and infrastructure layer and in the development tool chain, rather than reviewing them manually as part of the software delivery process.


**Further reading**:
* [DORA | DevOps Capabilities: Streamlining Change Approval](https://dora.dev/devops-capabilities/process/streamlining-change-approval/)