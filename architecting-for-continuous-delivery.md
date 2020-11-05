# Architecting for Continuous Delivery - Jez Humble

## Speaker

* Jez Humble
* [Continuous Delivery](https://continuousdelivery.com/)
* [Twitter](https://twitter.com/jezhumble)
* [LinkedIn](https://www.linkedin.com/in/jez-humble/)

## Video

* [Architecting for Continuous Delivery](https://www.youtube.com/watch?v=_wnd-eyPoMo)

<iframe width="840" height="472" src="https://www.youtube.com/embed/_wnd-eyPoMo"
frameborder="0"
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen>
</iframe>

## Source

* At [DevOps Enterprise Summit 2015](https://events.itrevolution.com/)

## Notes

If your architecture does not support continuous delivery then DevOps won't help.

So architecture and culture are the two biggest obstacles to achieve high performance continuous delivery and DevOps.

* Microservices are hard
* How to build Scalable maintainable reliable systems?

* What is continuous delivery?
* "The ability to get changes - features, configuration changes, bug fixes, experiments - into production or into the hands of users safely and quickly in a sustainable way."

* To be able to push out changes during normal business hours.

### Two golden rules

* Software (trunk, master, main) is always deployable.
* Everyone is checking into trunk (master, main) at least once a day.

### Ingredients

* Configuration management (setting up the environment, servers, etc.)
* Continuous integration  (everyone working on trunk (master, main), having a test suite that can check if everything works in a short amount of time and then fixing any breakage immediately)  Prioritizing fixing the
code over adding new features.
* Automated testing

### Deployment Pipeline

* If we are even slightly nervous when pushing the deploy button it means our automatic tests and validations are not good enough.

To validate the golden rules
* Testability (there is a good coverage of tests. "works on my machine" is not good enough)
* Deployability  (deployment is low-risk single pushbutton affair)

* [12 factor applications](https://12factor.net/)

* [Sam Newman: Building Microservices](https://www.amazon.com/Building-Microservices-Designing-Fine-Grained-Systems/dp/1491950358)

* But Microservices are not the only way to achieve Continuous Deployment.

* [Jess Robbins](https://en.wikipedia.org/wiki/Jesse_Robbins)
    * Master of disaster
    * Co-founder of [Chef](https://www.chef.io/)
    * Operations as a competitive advantage
    * "Operations at web scale is the ability to consistently create and deploy reliable software to an unreliable platform that scales horizontally."
    * [see](http://oreil.ly/1HRKUVE)
    * [see](http://radar.oreilly.com/2007/10/operations-is-a-competitive-ad.html)

* [CAP Theorem](https://en.wikipedia.org/wiki/CAP_theorem)

* component/service
* modularization: part of your system that could be swapped out for another implementation
* make system more maintainable (better encapsulation, lower coupling)
* [David Parnas](https://en.wikipedia.org/wiki/David_Parnas)
* [Law of Demeter](https://en.wikipedia.org/wiki/Law_of_Demeter)
* make system easier to build and test

* [Conway's Law](https://en.wikipedia.org/wiki/Conway%27s_law)

* [Rebecca Parsons](https://twitter.com/rebeccaparsons): "If you don't want your product to look like your organization, change your organization or change your product."

* Align your low bandwidth (human) communication boundaries with the APIs of your services.

* Splitting teams architectural basis.

### Two ways to bind the components together

* Bind components at Run Time (Microservices)
* Ken Exner ["Transforming Software Development"](https://bit.ly/1HxCEZy) (death start of Microservices from Amazon)
* Independent deplyment
* Don't break downstream! (Your team is responsible if any downstream users of your API breaks.)
* API versioning, AB testing etc.
* Monitoring

* Bind components at build time. (deploy a huge binary)
* A monolith


* John Penix
* [Large-Scale Continuous Testing in the Cloud](https://www.infoq.com/presentations/Continuous-Testing-Build-Cloud/)


* Michael T. Nygard
* [Release It!: Design and Deploy Production-Ready Software](https://www.amazon.com/Release-Production-Ready-Software-Pragmatic-Programmers/dp/0978739213)

* [Steve Yegge platform rant](https://bit.ly/1zxknpR)
* [other](https://gist.github.com/chitchcock/1281611)

* Werner Vogels, CTO of Amazon: ["you build it you run it"](https://bit.ly/11UJjmN)

* Strangler Application
* Start with user research!

* There is no "end state" of an architecture. Architecture will always change.

### DevOps Benchmarking
* Gene Kim
* Nicole Forsgren
* Jez Humble


![](assets/img/p/jez_humble.jpg)

