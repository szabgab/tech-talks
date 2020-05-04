# Testing in Production - Michael Bryzek

Production: Designing for Testability (aka. Testing in Production)
Is your code working in production? Right now? Does your monitoring system work? Does your alerting system work?

## Speaker

* Michael Bryzek
* [Twitter](https://twitter.com/mbryzek)
* [LinkedIn](https://www.linkedin.com/in/mbryzek/)
* [Gilt](https://www.gilt.com/)
* [Flow](https://www.flow.io/)

## Video

* [](https://www.youtube.com/watch?v=z-ATZTUgaAo)

<iframe width="840" height="472" src="https://www.youtube.com/embed/z-ATZTUgaAo"
frameborder="0"
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen>
</iframe>

## Source

* At [QCon 2017](https://www.infoq.com/presentations/quality-production/)

## Slides

## Notes




Verification in production is part of the developer experience.
Accountability, Devops, end-to-end ownership.
Software is testable.

True continuous delivery.
No staging environments.
Don't run your code locally.

Merging a pull-request gets deployed so the person who accepts the pull-request must be able to decide if it is ok to deploy this code. There is no QA or some other set of eyes looking at the code or verifying the product.

One way to do things - so no alternative way to deploy software or alternative way to test it.


No one likes their staging environment
* Bottleneck
* Fragile - because it is not treated as production
* Difficult to understand failure , especially if there are things that do not exist in production (but then I wonder why do they exist in staging?)
* Expensive (30-40% of budgets) ( I am really surprised)
* Creates the wrong incentives
* You still can't guarantee that deployment to production will work.

Don't run your code locally, write a tests.

If the organization decides that "call the tests pass" means the code is deployable, that puts the pressure on the developers to write the tests and to be able to rely on the tests. (side note: I still thing we need to have a place where we can look at the UI because I don\u2019t think I\u2019ll want to write tests for the UI. Especially not to check if it looks nice\u2026.)


Extreme Isolation - somebody else can't break your software

Even streaming (event bus)
Every Microservice has its own private database.


What is different in the production environment?
* The scale
* Maybe the <a href="https://en.wikipedia.org/wiki/Network_performance">network performance</a> (the throughput, the latency, \u2026 are different)
* Other things?

Create a bot to do things on the web site. (e.g. order a product) Have a specific domain for the bot to identify itself, and then they could easily identify the orders made by the bot and they could easily cancel those orders.


Production load testing.

When you work with a third-party API you have a contract with them (the API) and you respect that contract because they won\u2019t give a copy of their service to you.
SaaS even for internal accounts
API keys for sandbox accounts

A Sandbox is an identifier in production that is safe because the authors of the software made it safe.
The provider promises that if your code works with their sandbox then it will work with their production system as well.
A Sandbox account comes with no data just like a normal account, so a client can write their whole tests starting from the creation of the Sandbox account.

End to End Integration tests
* Create Sandbox org
* Run your tests
* Delete Sandbox org


* Their own [API proxy](https://github.com/flowvault/proxy)


Considerations
* Make production access explicit (not the default) (so environment variable or flag is needed, imho there should be no default envrionment)
* Use the API to test the software - just as the clients do.
* Restrict sensitive data (e.g. personal identifiable data, credit cards, etc.)
* Design for side effects (e.g. don't allow credit-cards to go to the bank in the testing or sandbox environments)


Automatically generate the documentation from the curl-based examples and responses. So the examples are always up-to-date.

* [API Builder](https://www.apibuilder.io/)
* Version control of APIs
* High Quality Mocks

* [Vivid Cortex](https://www.vividcortex.com/)
* Real Time  DB Monitoring

* Simple Alerts from Logs
* [Sumologic](https://www.sumologic.com/)
* [Splunk](https://www.splunk.com/)

![](assets/img/l/)

