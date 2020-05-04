# Architecting for Continuous Delivery - Jez Humble

## Speaker

* Jez Humble
* [Twitter]()
* [LinkedIn]()

## Video

* [](https://www.youtube.com/watch?v=_wnd-eyPoMo)

<iframe width="840" height="472" src="https://www.youtube.com/embed/_wnd-eyPoMo"
frameborder="0"
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen>
</iframe>

## Source

* At [Craft-Conf Budapest 2019](https://craft-conf.com/)

## Slides

## Notes

iIf your architecture does not support continuous delivery then DevOps won?t help.

So architecture and culture are the two biggest obstacles to achieve high performance continuous delivery and DevOps.

Microservices are hard
Scalable maintainable reliable systems

What is continuous delivery?
The ability to get changes ? features, configuration changes, bug fixes, experiments ? into production or into the hands of users safely and quickly in a sustainable way.


Be able to push out changes during normal business hours.

Two golden rules
?       Software (trunk, master,..) is always deployable
?       Everyone is checking into trunk (master) at least once a day

Ingredients
?       Configuration management (setting up the environment, servers, etc.)
?       Continuous integration  (everyone working on trunk, having a test suite that can check if everything works in a short amount of time and then fixing any breakage immediately)  Prioritizing fixing the
code over adding new features.
?       Automated testing

Deployment Pipeline

If we are even slightly nervous when pushing the deploy button it means our automatic tests and validations are not good enough.

To validate the golden rules
?       Testability (there is a good coverage of tests)
?       Deployability  (deploy is low-risk single pushbutton affair)


12 factor applications
https://12factor.net/

sam newman building microservices
https://www.amazon.com/Building-Microservices-Designing-Fine-Grained-Systems/dp/1491950358


https://en.wikipedia.org/wiki/Jesse_Robbins
master of disaster
co-founder of chef


operations as a competitive advantage
?Operations at web scale is the ability to consistently create and deploy reliable software to an unreliable platform that scales horizontally?
http://oreil.ly/1HRKUVE
http://radar.oreilly.com/2007/10/operations-is-a-competitive-ad.html


CAP Theorem
https://en.wikipedia.org/wiki/CAP_theorem


component/service
modularization

https://en.wikipedia.org/wiki/David_Parnas

https://en.wikipedia.org/wiki/Law_of_Demeter


Conway?s Law
https://en.wikipedia.org/wiki/Conway%27s_law

If you don?t want your product to look like your organization, change your organization or change your product?
Rebecca Parsons
https://twitter.com/rebeccaparsons

Align you low bandwidth (human) communication boundaries with the APIs of your services.

Splitting teams architectural basis.

Bind components at Run Time (Microservices)
Your team is responsible if any downstream users of your API breaks.
(API versioning, AB testing etc.)
Monitoring

Bind components at build time. (deploy a huge binary)


John Penix
Large-Scale Continuous Testing in the Cloud
https://www.infoq.com/presentations/Continuous-Testing-Build-Cloud/



Michael T. Nygard

Release It!: Design and Deploy Production-Ready Software
https://www.amazon.com/Release-Production-Ready-Software-Pragmatic-Programmers/dp/0978739213




steve yegge platform rant  bit.ly/1zxknpR
https://gist.github.com/chitchcock/1281611

werner vogels
you build it you run it

30:28



![](assets/img/l/)
