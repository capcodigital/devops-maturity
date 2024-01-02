[home](../README.md)
# [Development Practices](README.md) - Traceability In Version Control


There are many reasons that we need traceability within our version control system:

* **Audit and Security**: to prove that only authenticated and authorised users can and have made changes to the code
* **Bug Fixing**: to show when & how the bug was introduced - to aid fixing (and training)
* **Release Tagging**: to identify the code point that went into a particular release


## Commit messages

The following needs to be tracked as part of an effective version control

* **Who** made the change
* **When** was the change made (commited to the repository)
* **What** was changed
* **Why** was it changed

Although any good source control system automatically captures the **who**, **when**, and **what** - the **why** relies on the developer following good practice and writing meaningful comments in each and every commit.

The commit message should be:
* **Clear**: Comments like "fixed" or "small change" should be avoided.
* **Concise**: Keep commit messages to a short summary of the change. Aim for 70 characters or less.
* **Well Structured**: Having an agreed format can be helpful when reviewing code.
    * Starting the message with the ticket number is highly recommended*

\* Some source control (e.g. Bitbucket, GitHub) and work control (e.g. Jira) systems can be integrated to simplify going from a commit to a ticket, or to indicate which commits were made to action a ticket.


## Tagging

Tagging the repository is a handy method to easily identify key events in the code's history.

Examples of useful tags:

* a major change was introduced (e.g. "converted to NodeJS")
* the commit which was successfully built (e.g. "2.0.1", "2.0.1.5")
* the commit which was built and successfully deployed to production (e.g. "prod_20230904_1043", "release_ABC")
