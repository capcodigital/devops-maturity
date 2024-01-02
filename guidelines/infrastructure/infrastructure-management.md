[home](../README.md)
# [Infrastructure](README.md) - Infrastructure Management


Many organisations seek flexible technical infrastructure, often in the form of cloud computing. But there’s more to it than buying your infrastructure from a cloud provider. Five essential characteristics of cloud computing:

* **On demand self-service**: Consumers can provision computing resources as needed, without human interaction from the provider.
* **Broad network access**: Capabilities can be accessed through diverse platforms such as mobile phones, tablets, laptops, and workstations.
* **Resource pooling**: Provider resources are pooled in a multi-tenant model, with physical and virtual resources dynamically assigned on-demand. The customer may specify location at a higher level of abstraction such as country, state, or data center.
* **Rapid elasticity**: Capabilities can be elastically provisioned and released to rapidly scale outward or inward on demand, appearing to be unlimited and able to be appropriated in any quantity at any time.
* **Measured service**: Cloud systems automatically control, optimise, and report resource use based on the type of service such as storage, processing, bandwidth, and active user accounts.


Many organisations still use their traditional datacentre practices and processes to manage their cloud infrastructure, they can’t achieve the expected benefits, which according to DORA’s research include:

* Improved software delivery performance: faster throughput and higher levels of stability
* Better service availability
* Improved cost visibility: in 2019, we found that respondents who met all essential cloud characteristics are 2.6 times more likely to be able to accurately estimate the cost to operate software. They are also twice as likely to be able to easily identify their most operationally expensive applications.


**Infrastructure as Code**

Infrastructure as Code (IaC) is the managing and provisioning of infrastructure through code instead of through manual processes.

With IaC, configuration files are created that contain your infrastructure specifications, which makes it easier to edit and distribute configurations. It also ensures that you provision the same environment every time. By codifying and documenting your configuration specifications, IaC aids [configuration management](https://www.redhat.com/en/topics/automation/what-is-configuration-management) and helps you to avoid undocumented, ad-hoc configuration changes.

Version control is an important part of IaC, and your configuration files should be under source control just like any other software source code file. Deploying your infrastructure as code also means that you can divide your [infrastructure](https://www.redhat.com/en/technologies/management/ansible/infrastructure) into modular components that can then be combined in different ways through automation.

Automating [infrastructure provisioning](https://www.redhat.com/en/topics/automation/what-is-provisioning) with IaC means that developers don’t need to manually provision and manage servers, operating systems, storage, and other infrastructure components each time they develop or deploy an application.

Benefits:

* Cost reduction
* Increase in speed of deployments
* Reduce errors
* Improve infrastructure consistency
* Eliminate configuration drift
