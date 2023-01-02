# Prioritizing Technical Debt as If Time & Money Matters - Adam Tornhill

## Speaker

* [Adam Tornhill](http://adamtornhill.com/) founder of [Codescene](https://codescene.com/)

## Video

* [video](https://www.youtube.com/watch?v=w9YhmMPLQ4U)

<iframe width="840" height="472" src="https://www.youtube.com/embed/w9YhmMPLQ4U"
frameborder="0"
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen>
</iframe>

## Source

* At [GOTO 2022](https://gotoams.nl/2022)


## Software development at scale

Lehman's "Laws" of Software Evolution

[Lehman, M.M. (1980) Programs, Life Cycles, and Laws of Software Evolution. Proceedings of the IEEE, 68, 1060-1076.](https://ieeexplore.ieee.org/document/1456074)


## Continuing Change

* "a system must be continually adapted or it becomes progressively less satisfactory"

* A successful software is never done.

## Increasing Complexity

"as a system evolves, its complexity increases unless work is done to maintain or reduce it"

## Increasing Complexity: consequences and impact

### Impact on the Roadmap:

* Cycle times get longer and longer: A feature that would have taken 1 week a year ago, now takes a month to implement.
* Longer cycle times means less predictability. Software estimation was always a black art, with complexity it gets harder.

### Impact on the team:

* higher turnover rate - working on unnecessarily complex stuff is not fun.
* key person dependencies, only one person know certain areas of the code (lower bus factor).

### Impact on the users:

* bugs. lots of bugs.
* aka. lower quality

## Quantifying Technical debt

* Quantifying Technical debt via static analysis

Example: tried at a client on a 15 year old code-base. The tool reported 4,000 years technical debt. (It is unclear to me what this really means)

Conclusion: Quantifying technical debt is depressing, but it isn't actionable as we cannot possibly invest that much time and money in the project.

Technical debt cannot be prioritized based on the code alone. The impact on the business is the interesting part.
How much extra time is needed to develop a new feature because of the technical debt. This is something that cannot be measured from the existing code.

There is always a trade off between improving existing code and adding new features.

* [Software Design X-Rays](https://pragprog.com/titles/atevol/software-design-x-rays/)

## Behavior Code Analysis = code + people + context

* Version Control - A behavioral Data Source

The source code of Android: [platform framework base](https://android.googlesource.com/platform/frameworks/base.git)

* 3 million lines of code
* 2.1 million lines of Java
* 2,000 developers


Code complexity - how hard it is for a human to understand the code - but it is the least interesting metric because it only matters when we have to deal with it.

What is more important is frequency of changes (commits) in an area of code.

Actually the really problematic code is the complex code that we have to change often.


## Complexity explained: is "code quality" really a thing?

"The assumption that fundamentally different views of complexity can be characterized by a single number is counter to the fundamental concepts of measurement theory."

"the most promising approach is to identify attributes of complexity and measure these separately"
[Software Measurement: A Necessary Scientific Basis](https://www.researchgate.net/publication/3187630_Software_Measurement_A_Necessary_Scientific_Basis)


There is no such thing as "code complexity" (as a single number)

## Healthy code: Beyond a single metric

Identify 20-25 different factors, depending on programming language.

* [Measure the Code Health of your Codebase: a continuous feedback loop for engineering decisions based on data](https://codescene.com/blog/measure-code-health-of-your-codebase)

Module level:

* Low cohesion
* Brain classes

Function level:

* Brain methods
* Copy-pasted logic

Implementation level:

* Deeply nested logic
* Primitive Obsession


Finding bad code is easy. Finding which part to fix is hard.


## X-Ray

* Change frequency
* Linex of code
* Cyclomatic complexity

## Tech Debt and People

* Legacy Code and Technical Debt are not the same

* Legacy Code (many definitions, one of them is)
    * lacks in quality
    * we did not write ourselves

* Making legacy code: what is the impact if one of the people working on the code leaves? It depends how much of the code-base they wrote.
In each team there are only a few people who write most of the code. If they leave and noone knows that part of the code-base it can easily become "legacy code".
Certainly it is code that noone knows. This is known as the "bus factor".

## Mitigate off-boarding risks

That is when one of the contributor leaves.

There are 3 factors:

* knowledge loss when a person leaves
* relevance (hotspot) - how often that part of the code changes
* impact (complexity) - how complex is that part of the code

knowledge loss + relevance (hotspot) + impact (complexity)


## There is more to Code Complexity than just the Code

* Social factors influence how we perceive a codebase

