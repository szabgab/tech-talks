# Continuous Delivery by Martin Fowler

## Speaker

* [Martin Fowler](https://martinfowler.com/)
* [Twitter](https://twitter.com/martinfowler)

## Video

* [Continuous Delivery by Martin Fowler](https://www.youtube.com/watch?v=aoMfbgF2D_4)

<iframe width="840" height="472" src="https://www.youtube.com/embed/aoMfbgF2D_4"
frameborder="0"
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen>
</iframe>

## Source

* At []()

## Slides

## Notes


Continuous Delivery is in the Agile Manifesto
Kent Back was already doing.

Deployment Pipeline - a series of tests (starting by the question, is this code even compile) to determine if the new version of the code is usable.
For small project it might be a one-step system, for bigger project it will likely be a multiple-step system.


Be able to confidently send the code into production.

Continuous Delivery vs Continuous Deployment


Continuous Deployment = every changes gets deployed to production.

Continuous Delivery = is broader, we get to the point where we can deploy, but we don't necessarily do it.

Technical team is done: it is the delivery.
Business team makes the decision if deploy or not.


Automation: Build, Testing, Deploy

Everything must be in Version Controls
* Source code
* Database schema
* Deployment scripts
* Code to deploy servers


DevOps = a cultural phenomenon
* Developers have to think about Operations
* Operations people have to think about Developers
* It is a communication and cultural shift.

Continuous Integration: Everyone integrates their work with everyone else frequently?

* Does everyone on the team commit to the mainline trunk (master) at lest once a day?
* Do you have a solid battery of tests that you can feel confident your code is ready for production?
* If you have a production failure will it be fixed within 10-20 minutes?

Benefits of Continuous Delivery:
- Lowering deployment risk    (small changes, be able to roll back)
- Sense of real progress (what does "done" really mean? works on the developers computer? does it deliver value?)
- User feedback (don't listen to what they say they want, monitor what they do and learn from that.)


[Continuous Delivery: Reliable Software Releases through Build, Test, and Deployment Automation](https://www.amazon.com/Continuous-Delivery-Deployment-Automation-Addison-Wesley/dp/0321601912) by
Jez Humble and David Farley

![](assets/img/l/)



