[home](../README.md)
# [Continous Delivery](README.md) - Source Control


Having a secure and robust source control system is key tool to ensure that the team can keep track of changes to the code over time. Just like every tool at our disposal, how that tool is used is everything.

If there are no clear rules and processes for the team to follow, a source control system will quickly get out of hand and the team's ability to deliver change will be severely hampered.

## Selecting the right source control system

Some of the popular tools include:
* [GitHub](https://github.com/)
* [Bitbucket](https://bitbucket.org/product/)
* [GitLab](https://bitbucket.org/product/)
* [Mercurial](https://www.mercurial-scm.org/)
* [AWS CodeCommit](https://aws.amazon.com/codecommit/)
* [Azure Repos](https://azure.microsoft.com/en-us/products/devops/repos)
* [GCP - Cloud Source Repositories](https://source.cloud.google.com/onboarding/welcome)

There is no "one size fits all" answer here. Things to consider include:
* **Intergration**: how well does the tool integrate with exising tools like IDE, CI/CD engine, work tracking system
* **Hosting options**: is it available in your preferred on prem/cloud
* **Cost**:
* **Bundling**: does it come as included with this other tool that you require

## Getting the most out of a source control system

* Select the right [branching strategy](../development-practices/branching-strategy.md)
    * Ensure that all team members are fully trained and engaged
    * Depending on the strategy, enable branch restrictions to prevent protected branches from being corrupted
* Make code reviews the norm
* Plug the system into your build pipeline so that commits trigger builds
* Teams that focus on only pushing/merging quality code, spend less time "fixing the build"
    * Ensure that the changes will not fail the automated tests by running them locally before committing
* Creating changes behind feature toggles so that they can be integrated into an environment in a disabled state
* Deleting branches once they have been merged
* [Tagging](../development-practices/traceability-in-version-control.md#tagging) key points in the history of the code




---
**Further reading**:
* [The Pros, Cons, and Best Practise for using Feature toggles](https://www.split.io/blog/the-pros-cons-and-best-practices-for-using-feature-toggles)
