[home](../README.md)
# [Continous Delivery](README.md) - Build Reliability

Broken or failing builds in a CI/CD pipeline can deteriorate a team's faith in its own processes. It can also hinder a team's ability to efficiently deliver high-quality software. That's why it's important to identify and fix broken builds in a CI/CD pipeline.

These types of CI/CD challenges aren't unique to any specific tool. Broken builds can be red flags for larger issues and signify impediments to current -- and future -- workflows. Luckily, there are best practices to remediate broken builds and avoid failing ones.

Tips or pointers to help remediate broken builds:

**Make sure it builds locally**

Like the classical saying of “have you tried turning it on and off again”, making sure you can run and build a solution locally in a similar way to the way the build agent executes a build will give developers a higher degree of success when trying to quickly identify issues with a build. For example, a build fails but locally it is working, it could be as simple as a dependency on a file that was forgotten to be checked in etc.

**Ensure sufficient logging on the build server**

Ensuring that you have verbose logging, showing every step of the way will aid developers in pinpointing the exact step/location the error is taking place. Cutting back on time a developer will need to spend to investigate what is going wrong.

**Have a way of inspecting the file system**

Often issues related to configuration come from a missing configuration file or a hanging file from a previous build. Exposing the workspace where the build takes place can help identify this type of issue. If this is the case, running a clean build can often remediate the issue. DevOps tools often have functionality to expose this to the developer who is investigating (e.g., Jenkins has a workspace folder a user can access from within the tool).

**Implement Alerts**

By implementing ChatOps you can reduce the amount of build failures that happen for a given solution. ChatOps allows you to alert and send targeted communications to relevant individuals. Often an alert gets configured for failing builds in a shared communication channel (teams/slack), this allows a quick feedback loop to inform the developers when something isn’t going as expected.
