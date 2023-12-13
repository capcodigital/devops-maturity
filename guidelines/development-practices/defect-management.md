[home](../README.md)
# [Development Practices](README.md) - Defect Management


Effective defect management is crucial to ensure that issues are fixed in an appropriate timeframe. There are many tools available to track issues (e.g. Jira) and recording issues in the same tool as jobs are assigned enables them to be prioritised together with other work.


## Discovery

When recording a bug it is important to capture:
* **Definition of bug**: e.g. Surname case logic not working in all cases
* **Steps to recreate bug**: e.g. Create a new contact with surname of o'donnell and click save
* **Expected behaviour**: e.g. Surname should be displayed as "O'Donnel"
* **Actual behaviour**: e.g. Surname is be displayed as "O'donnel"
* **Additional information**: e.g. Other failing cases include "McEnroe" and "MacDowell"
* **Evidence**: e.g. Screenshot with issue highlighted


## Triage

The bug report would need to be reviewed in order to:
* **Confirm it is a bug**: some reported bugs are actually desired functionality e.g. in this case, it is correct that input box be disabled due to the particular product options selected
  * In the circumstances where there remains disagreement on whether the reported bug is or is not a bug, a senior member of the team would need to decide (e.g. product owner, test manager)
* **Set priority**: Is this a production-breaking issue that must be fixed within the hour or is it a very rare and minor inconvience that can be added to the backlog


## Fixing and Closing the defect

Regardless of the severity of the bug, once it has been fixed, it needs to be verified and accepted as fixed.
The bug tracker needs to be updated to show closure.

There can be times when a fix gets rejected multiple times. This can lead to increased tension within the team and should be resolved promptly to maintain [team health](../culture/team-health.md).


## Defect Metrics

Having an effective defect management process can enable improvements:
* **Defect Distribution**: does a particular step in the user journey have a disproportionate level of bugs - does it require a review/re-engineering?
* **Defect Rejection Rate**: a high level of rejected defects could indicate that those raising the issues would benefit from addtional training on the expected functionality
* **Number of times a fix was rejected**: repeated fix rejections could indicate that those fixing the issues would benefit from addtional training on the expected functionality 
* **Time taken to resolve**: see also [Mean Time to Restore](mean-time-to-restore.md)


---
**Further reading**:
* [What is Defect Clustering in Software Testing?
](https://www.browserstack.com/guide/defect-clustering-in-software-testing)
* [How to write effective software defect reports](https://techbeacon.com/app-dev-testing/how-write-effective-software-defect-reports)
