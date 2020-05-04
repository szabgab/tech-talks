# 10+ Deploys Per Day: Dev and Ops Cooperation at Flickr - John Allspaw, Paul Hammond

## Speakers

* John Allspaw ran the Operations group at [Flickr]( https://www.flickr.com/)
* [John Allspaw Twitter](https://twitter.com/allspaw)
* [John Allspaw LinkedIn](https://www.linkedin.com/in/jallspaw/)

* Pauk Hammond ran the Engineering group at [Flickr]( https://www.flickr.com/)
* [Paul Hammond Twitter](https://twitter.com/ph)
* [Paul Hammond LinkedIn](https://www.linkedin.com/in/paulhammond/)

## Video

* [10+ Deploys Per Day: Dev and Ops Cooperation at Flickr](https://www.youtube.com/watch?v=LdOe18KhtT4)

<iframe width="840" height="472" src="https://www.youtube.com/embed/LdOe18KhtT4"
frameborder="0"
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen>
</iframe>

## Source

* At [Velocity 2009](https://conferences.oreilly.com/velocity)

## Slides

## Notes

How Development and Operations fit together.

Devs. vs Ops.

Stereotypes:
* Operations are like old grumpy men who always say

Traditional roles:
* Dev's job is to add new features
* Ops' job is to keep the site stable and fast


* The reality is that *Ops job is to enable the business*
* The business requires change
* Change is the root cause of most outages.

Two options:
* Discourage change in the interest of stability
* Build tools and culture to Allow change to happen as often as it needs to

Build tools to Reduce the risk of changes.
Build tools to be able to easily recover from failures

Developers who think more like operations people
Operations people who think more like Developers.

1. Automated infrastructure -> consistent platforms for development and production (Infrastructure as code?, Role and configuration management)
2. Shared version control for both development and operations
3. Set up a one step build system  (build and deploy to staging)
4. One step deploy
5. Have a deploy log (Who? When? What?)

(Continuous Integration / Continuous Deployment)

[Hudson (now Jenkins)](https://jenkins.io/)

Each individual deploy involves less change and thus less risk.

### Feature flags

Always ship "trunk" (what is usually called "master" in Git)

(They) don't work in branches, but use feature flags to enable/disable certain feature of the application / web site.

Allow private beta on productions servers.

This Allows bucket testing (A/B testing)
Turn on a features to a subset of the users.
Allows dark launches.

This takes the fear out of the work.
They had a couple of hundred feature flags.

Some of these flags are on/of, others are more gradual knobs.

### Shared metrics

* Developers have access the metrics of the operation and application level metrics in one place.
* Show the last site update on the top of every page of every metric in order to have better context.

### Adaptive feedback loops

### Communication

* IRC ad IM bots (it could be also Slack or Microsoft Team)

### Culture
Argumentative, combative culture won?t help?.
Having a culture of respect
Don?t stereotypes (Not all developers are lazy, not all ops people are grumpy)
Everyone is a snowflake
Respect the opinions of other people and the responsibilities of other people that means people have different priorities.
Don?t just say ?no?. Try to find out what problem they are trying to solve.

Developers and Operations come together to find unique solutions.
Don?t hide your solutions from the other people

Developers: Talks to the ops about the impact of your code!
What metrics will change, and how  (CPU, memory ?)
What are the risks
What are the signs that something is going wrong
What are the contingencies

## Trust

Provide knobs and levers that in operation can be tweaked to
Ops: Be transparent, give devs (read only) access to the system so they can see what?s going on without going through operations.
Its low risk and empowering.
They can access all the metrics.

## Healthy attitude about failure:
Failure will happen
Think about what to do when failure happens (evacuation plans)
Ability to respond to problems
Fire-drills to prepare for the real fire (real problem)

Avoiding blame, rule of no finger-pointing.

If there is a problem, first fix it and only feel bad about it.

Developers: Remember that someone else will probably get woken up when your code breaks. (better yet, make the developers on-call. Wake them up when the code breaks. Put Devs on call.)

Developers: What would you do differently if there was no one else who could fix the issues when they break in the middle of the night? What would you do differently if it was you who get woken up?

Operations: provide constructive feedback on what?s going on. What are the current aches and pains.

1. Automated infrastructure
2. Shared Version control
3. One step build and deploy
4. Feature Flags
5. Shared metric
6. IRC and IM robots


1. Respect
2. Trust
3. Healthy attitude about failure
4. Avoiding Blame



![](assets/img/l/)
