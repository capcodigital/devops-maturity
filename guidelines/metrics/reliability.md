[home](../README.md)
# [Metrics](README.md) - Reliability


When applications are reliable, there are fewer bugs and issues that need addressing, less time is required to maintain the application and therefore the team are able to spend more time on quality improvments - be it, delivering new functionality or focusing on their own DevOps maturity.


Being able to turn to a dashboard to demonstrate an application's reliability is extremely powerful. It gives you an invaluable incite into how the application is performing and can be used to predict things like future performance based on organic customer growth or whether the application could cope with a sudden influx of request following a planned product launch.


Here is a start on just some of the things that could be measured:

* **Error messages being output to logs**: All error messages should indicate an issues that needs investigating. If you have an error message that indicates something else - is recording it an error the best approach? Schedule refactoring this into a future sprint's technical debt time.
* **Response Time**: Having an accurate historical record of how long your application takes to service requests can be used to:
** Highlight improvement/degredation of performance following implimentation of a new feature
** Identify your application's peaks and troughs - allowing fine tuning of cloud resourcing (or similar)
** Recognise performance bottlenecks
** Demonstrate the need for investment in an improved hosting solution etc.
* **CPU and Memory Usage**: If your application regularly uses most of its allocated resources, how can it be expected to cope with the inevitable spike?


On top of the above non-exhaustive list of things to measure, it is well worth putting time into capturing the experience of those who are actually using the application on a day to day basis.
Your automated metrics may always be "in the green", but if the users are regularly reporting performance issues - there may be something missing in your dashboard. It may also be an indicator that what was considered "good performance" is no longer keeping up with the customer's expectations.


**Dashboards vs. Alerts**

There is no simple answer for how best to present reliability metrics. In an ideal world, when everything is reporting "green", we shouldn't be distracted from what we are doing. When things start to "go wrong", we want to be informed with enough time to fix it before anyone notices.
A dashboard on a screen in the corner of the office is all well and good - but it needs people to take notice and act when required.
An over-reliance on alerts (email/sms/dm) can easily lead to alert-fatigue.
As with many things in life - finding the right balance is key.
