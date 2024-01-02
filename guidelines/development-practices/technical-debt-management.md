[home](../README.md)
# [Development Practices](README.md) - Technical Debt Management


## What is Technical Debt

The first thing to acknowledge is that, since there is no such thing as a perfect system, **technical debt is unavoidable**.

Technical debt (tech debt) is the accumilation of a system's imperfections. This can take many forms, including:

* **Aging infrastructure**: when commissioned, the infrastructure may have been fit for purpose but can it still cope with the increased traffic or growing workload? Not to mention keeping up to date with software patches.

* **Code which is difficult to maintain**: possibly the original authors have moved on or maybe the code was not written in an optimal manner.

* **Code base which is written in different language/frameworks**: languages and frameworks evolve and fall out of favour.

There may be times when a delivery deadline requires the team to agree to add to its tech debt but this needs to be the exception to the norm and this debt needs to be addressed ("paid back"). In a similar manner to financial debt, unless tech debt is managed carefully, it will grow and hamper the team's ability to deliver.

Keeping on top of tech debt takes time and effort and must be balanced with the need to deliver change. Too much focus on one or the other will have issues in the long run.

## Avoiding Technical Debt

The less tech debt that added to a system, the less that has to be fixed down the line.

Regular code reviews and Paired Programming (AKA. Extreme Programming) are good approaches to identify and fix tech debt before it makes it into the system.

Investing time into identifying potential tech debt is an effective way to share knowledge between senior and junior team members as well as sharing new ways of doing things.

## Tracking Technical Debt

Like tracking defects, effective tech debt management is crucial to ensure that issues are fixed in an appropriate timeframe. There are many tools available to track issues (e.g. Jira) and recording issues in the same tool that jobs are assigned, enables them to be prioritised alongside other work.

## Fixing Technical Debt

Whilst having dedicated time/sprints for the team to focus on addressing tech debt is a common approach, it is often an after thought and this time is frequently the first to be sacrificed when time is tight.

Far better is to make it part of the team's normal working strategy. Even if the ticket that the developer has picked up isn't a dedicated tech debt ticket, they always have a mind of how to improve the overall code base whilst making their change.
