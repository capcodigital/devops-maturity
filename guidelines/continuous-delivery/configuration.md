[home](../README.md)
# [Continous Delivery](README.md) - Configuration


Configuration management helps engineering teams build robust and stable systems using tools that automatically manage and monitor updates to configuration data. Complex software systems are composed of components that differ in granularity of size and complexity. For a more concrete example consider a microservice architecture. Each service in a microservice architecture uses configuration metadata to register itself and initialize. Some examples of software configuration metadata are:

* Specifications of computational hardware resource allocations for CPU, RAM, etc.
* Endpoints that specify external connections to other services, databases, or domains
* Secrets like passwords and encryption keys


How to implement configuration management:

**Identification**

The first action towards configuration management is information gathering. Configuration data should be aggregated and compiled from different application environments, development, staging, and production for all the components and services in use. Any secret data like passwords and keys should be identified and securely encrypted and stored. At this point configuration data should be organized into data files that can be pointed to as a central source of truth.

**Baseline**

After configuration data has been aggregated and organized a baseline can be established. A baseline configuration is a known state of configuration that will successfully operate the dependent software without error. This baseline is usually created by reviewing the configuration of a functioning production environment and committing those configuration settings.

**Version Control**

Your development project should use  a version control system. If not, install Git, initialize a repository for the project, and add the configuration data files to the repository. A word of caution before adding configuration data to a repository: make sure that any secret data like passwords or keys are encrypted with an external key. Secret data accidentally committed to a repository is a huge risk. It needs to be scrubbed from the repositories history or it will be at risk of being exploited.

**Auditing**

Having configuration data organized and added to a repository enables collaboration and visibility into the system’s configuration. The popular pull request workflow that software teams use to review and edit code can then be applied to configuration data files. This helps build out an audit and accounting system. Any changes applied to the configuration must be reviewed and accepted by the team. This adds accountability and visibility into configuration changes.


Read more here: [Configuration management: definition and benefits](https://www.atlassian.com/microservices/microservices-architecture/configuration-management)