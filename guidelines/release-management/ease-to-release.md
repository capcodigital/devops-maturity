[home](../README.md)
# [Release Management](README.md) - Ease To Release


There are a number of practices that can be introduced to help with ease to release and positively impact on reducing deployment pain and burnout.

The following scenarios in a production release are classified as painful situations that can lead to burnout:

1. Everyone involved is stressed out.
1. Releases happen after hours, often on weekends, or in the early-morning hours.
1. You have several error-prone manual steps that everyone needs to follow.
1. Your team relies on a "deployment hero," one person who actually knows how to get the code deployed.
1. You launch every release with a silent prayer — you hope it works, but you’re not really sure it will.
1. Users are often negatively affected by new releases.
1. Releases are infrequent, occurring only a few times a year.


By embracing a DevOps culture and some DevOps good practices we can reduce this deployment pain and mitigate the risk that a change into production can bring

1. **Use infrastructure as code (Iac)**: IAC describes your infrastructure in source files that you check into version control and applying them automatically. IAC offers three key advantages: more reliable releases, more repeatable release process and represents living documentation of your infra improving audits.
1. **Destroy all your servers all the time**: Configuration drift is when the configuration of a server evolves over time, due to the compound effect of making changes on top of existing changes. The only remedy for configuration drift is to destroy your servers on purpose and recreate them. This technique will force you to ensure that your infrastructure code actually contains an accurate description of how your server needs to be configured
1. **Introduce zero downtime deployments**: Use Blue-Green Deployments or Canary deployments in order to Release software without affecting your users and allow to do a fast rollback in case of failure
