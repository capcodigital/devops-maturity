[home](../README.md)
# [Infrastructure](README.md) - Architecture


Whether you’re using Kubernetes or mainframes, your architecture enables teams to adopt practices that foster higher levels of software delivery performance.

When teams adopt continuous delivery practices, adopting the following architectural practices drives successful outcomes:

* Teams can make large-scale changes to the design of their systems without the permission of somebody outside the team or depending on other teams.
* Teams are able to complete work without needing fine-grained communication and coordination with people outside the team.
* Teams deploy and release their product or service on demand, independently of the services it depends on or of other services that depend on it.
* Teams do most of their testing on demand, without requiring an integrated test environment.
* Teams can deploy during normal business hours with negligible downtime.


Given the pros and cons of architectural archetypes, each fits a different evolutionary need for an organization.

| Archetype | Pros | Cons |
|---|---|---|
| **Monolithic v1**<br><br>(all functionality in one application) | <ul><li>Simple at first</li><li>Low interprocess latencies</li><li>Single codebase, one deployment unit</li><li>Resource-efficient at small scales</li></ul> | <ul><li>Coordination overhead increases as team grows</li><li>Poor enforcement of modularity</li><li>Poor scaling</li><li>All-or-nothing deploy (downtime failures)</li><li>Long build times</li></ul> |
| **Monolithic v2**<br><br>(set of monolithic tiers: frontend presentation, application server, database layer) | <ul><li>Simple at first</li><li>Join queries are easy</li><li>Single schema deployment</li><li>Resource-efficient at small scales</li></ul> | <ul><li>Tendency for increased coupling over time</li><li>Poor scaling and redundancy (all or nothing, vertical only)</li><li>Difficult to tune properly</li><li>All-or-nothing schema management</li></ul> |
| **Microservice**<br><br>(modular, independent, graph relationship or tiers, isolated persistence) | <ul><li>Each unit is simple</li><li>Independent scaling and performance</li><li>Independent testing and deployment</li><li>Can optimally tune performance (caching, replication, etc.)</li></ul> | <ul><li>Many cooperating units</li><li>Many small repos</li><li>Requires more sophisticated tooling and dependency management</li><li>Network latencies</li></ul> |

 

**Common pitfalls in architecture**

* **Simultaneously releasing many services**: In teams where testability and deployability are not prioritized, most testing requires the use of complex and expensive integrated environments. In many cases, deployments require that you simultaneously release many services due to complex interdependencies. These “big-bang” deployments require teams to orchestrate their work, with many hand-offs and dependencies between hundreds or thousands of tasks. Big-bang deployments typically take many hours or even days, and require scheduling significant downtime.
* **Integrating changes with the changes from hundreds, or even thousands, of other developers**: Those developers, in turn, might have dependencies on tens, hundreds, or thousands of interconnected systems. Testing is done in scarce integration test environments, which often require weeks to obtain and configure. These environments are typically not representative of production, reducing the value and accuracy of the testing. The result is not only long lead times for changes (typically measured in weeks or months) but also low developer productivity and poor deployment outcomes.
* **Creating bottlenecks in the software delivery process**: Example bottlenecks could be a single team that many others rely on either from a manual process standpoint (testing, deployment, and so on) or from a service operation standpoint. In both examples, those bottlenecks create single points of failure and demand that those teams or services scale to meet the demands of the many dependent teams.


**Loosely coupled architecture**

The separation of concerns to this date, it is arguably the single most important rule in software design. From an architectural point of view systems with high cohesion and low coupling would automatically have separation of concerns, and vice versa.

Modular systems are designed based on the principles of high cohesion and low coupling, on which small changes would most likely affect only a single module. Deploying the change will impact less to the entire application and it will require a shorter process to deploy it to production, reducing the risk and impact of the change.


Benefits:

* Clear Definition of purpose of use
* Reduce close coordination among modules
* Enabler of autonomous multi-feature teams
* Enabler for Feature team scalability
* Multi-language support at programming level
* Independent and more granular scaling
* More flexible hardware/software infrastructure
* Reduce Risk and impact of Change
* Increase frequency and lead time of deployments
* Reduced Time to Market
* Improve release stability
* Improve service recovery times in the event of an outage


Domain driven design – approaches and principles

* **Capture the domain model, in domain terms, through interactions with domain experts**. In other words, talk to the people in the businesses where you are solving problems and understand them from their point of view first and foremost. This is how you form the ubiquotous language of the domain and set the foundation for harmonious models.
* **Embed Domain terminology in the code**. This means naming things the way the domain expert would name them, including classes, methods, commands, and especially domain events. This is how you reflect the domain model in the code.
* **Protect the domain knowledge from corruption by other domains, technical subdomains, etc**. If you find that your code is talking about two different things—e.g., the domain solution and the technical implementation—separate those components to keep the subdomains apart. This strategy tends to result in classes with single responsibilities and a terse, focused vocabulary. Put "translators" at the boundaries (anti-corruption layers) between subdomains to keep them from depending on each other’s structures unnecessarily, and also to prevent blurring of the meaning of domain terms.


More information:

[DevOps Capabilities: Loosely Coupled Architecture](https://dora.dev/devops-capabilities/technical/loosely-coupled-architecture/)
