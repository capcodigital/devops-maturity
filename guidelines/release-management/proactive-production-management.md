[home](../README.md)
# [Release Management](README.md) - Proactive Production Management


**Chaos Engineering**

Chaos Engineering is the discipline of experimenting on a distributed system in order to build confidence in the system’s capability to withstand turbulent conditions in production.

To specifically address the uncertainty of distributed systems at scale, Chaos Engineering can be thought of as the facilitation of experiments to uncover systemic weaknesses.  These experiments follow four steps:

1. Start by defining ‘steady state’ as some measurable output of a system that indicates normal behaviour.
1. hypothesise that this steady state will continue in both the control group and the experimental group.
1. Introduce variables that reflect real world events like servers that crash, hard drives that malfunction, network connections that are severed, etc.
1. Try to disprove the hypothesis by looking for a difference in steady state between the control group and the experimental group

The harder it is to disrupt the steady state, the more confidence we have in the behaviour of the system.  If a weakness is uncovered, we now have a target for improvement before that behaviour manifests in the system at large

![Chaos Experiment](../../images/proactive-production-management-chaos.png)


Chaos Engineering Principles

* **Build a Hypothesis around Steady State Behaviour**: By focusing on systemic behaviour patterns during experiments, Chaos verifies that the system does work, rather than trying to validate how it works.
* **Vary Real-world Events**: Chaos variables reflect real-world events.  Prioritise events either by potential impact or estimated frequency.  Any event capable of disrupting steady state is a potential variable in a Chaos experiment.
* **Run Experiments in Production**: Systems behave differently depending on environment and traffic patterns.  Since the behaviour of utilisation can change at any time, sampling real traffic is the only way to reliably capture the request path.  To guarantee both authenticity of the way in which the system is exercised and relevance to the current deployed system, Chaos strongly prefers to experiment directly on production traffic.
* **Automate Experiments to Run Continuously**: Running experiments manually is labor-intensive and ultimately unsustainable.  Automate experiments and run them continuously.  Chaos Engineering builds automation into the system to drive both orchestration and analysis.
* **Minimise Blast Radius**:  Experimenting in production has the potential to cause unnecessary customer pain. While there must be an allowance for some short-term negative impact, it is the responsibility and obligation of the Chaos Engineer to ensure the fallout from experiments are minimised and contained.


---
**Further reading**:
* [Principles of chaos engineering](https://principlesofchaos.org/)
