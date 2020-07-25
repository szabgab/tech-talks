# Scaling Engineering by Hacking Conway's Law - Aviran Mordo

## Speaker

* Aviran Mordo VP of Engineering at o[Wix.com](https://wix.com)
* [Twitter](https://twitter.com/aviranm)
* [LinkedIn](https://www.linkedin.com/in/aviran/)

## Video

* [Scaling Engineering by Hacking Conway's Law](https://www.youtube.com/watch?v=UYc2RNcjLRw)

<iframe width="840" height="472" src="https://www.youtube.com/embed/UYc2RNcjLRw"
frameborder="0"
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen>
</iframe>

## Source

* JAX London Conference 2020

## Notes

* [Wix](https://www.wix.com/)
* Growing the engineering team while growint the company from 100 to 1000 people in 5 years.
* 2 teams (back-end team, front-end team 5-10 people in each team)
* Good at delivering the new and shiny new product, but old products got neglected. Because we were shifting resources (aka. people) to new projects.

* Functional unit model (where Wix was)
* Business unit model (Google has)  silos, everyone works on their own product/project.

* At Wix people were constantly jumping from one project to another.


### Assumptions at 7:45

* There is no perfect model.
* It depends on the company's current challanges, life cycle phase and culture.
* Every model should be tuned constantly and evolve with the company.


### Wix's Gangs and Guilds model

* A Guild is a group of people that share expertise, knowledge, tools, code, and practice. (horizontal ??)
* Gangs (were feature teams)o

No silos

* Gang: what to do
* Guild: how to do


* Gangs have a "Team lead" or "Product lead" and Team Members
* Guilds have "Guild Manager/Guild Leader" and "Guild Master" (Bummble bees), Guild infra team


* All the infrastructure concerns are part of the guilds - the tech stack.

* Hiring to guilds and not into the gangs. This increased the quality of new hires.
* Compensation is set by the guild.

* The success of the Guilds and the Guild managers are measure by the success of the feature teams.

### Back-end Guilds at Wix:

* Java and Scala
* NodeJS

* Guilds at Wix were created about the same time as in [Spotify](https://www.spotify.com/) but they are different from those.


At one point (around 800 people) they notice they have too many gangs and guilds and it was hard to manage.
So they created "Companies" that are clusters of Gangs with a "CEO". They can operate independently as a startup.
Some companies are small (4 people) some have 100 people.

Unfortunately this created product silos.

* By creating small rooms where 4-10 people can sit, they limited the sizes of their teams.

* By creating Microservices you allow yourself to use any technolgy stack you like. Which would be a huge mistake.
In order to scale as an org you need to limit the technologies to a few.

### Limit your stack = shareing knowledge

* Code reuse
* Cross cutting concerns (session, security, auditing, testing, logging, ...)
* Faster system evolution
* Development velocity

* Over 1000 unique microservices
* Deploying 300 times a day
* A single team can own 1-5 microservices

### Culture beats process every time - ROQS

* Responsibility
* Ownership
* Quality
* Sharing

* Dev-Centric culture - Involve the developer
* TDD is the key - they don't enforce TDD, but the guilds are teaching it and if you don't use it you might take production down which is a bad thing. They do require testing however.

* When there is a bug in production, the first question asked in a post-mortem is where is the test that covered this scenario.


### Quality

* To have Quality (of code and product) you need Better Engineers.
* To have Better Engineers you need to grow them. You need Professional Growth.
* To have Professional Grows you need investment in People and Training.

### Guild Day - 20% of the time dedicated to education and personal growth

* Engineers work 4 days a week with their company (gang).
* Thursday is Guild day.
* Developers conduct quality enhancing activities with the Guild.


### Guild Week - Game of Gangs

* One week each quarter
* Pair programming with a person from another company (inside Wix)

* Goal #1 - Improve engineering skills and quality

### Communication channels

* monday.com
* Slack
* Stackoverflow
* WixAnswers
* confluence
* whatsapp
* Gmail

### Elements of healthy growth

* Transparency
* Quality
* Trust and Collaboration
* Independence
* Growth
