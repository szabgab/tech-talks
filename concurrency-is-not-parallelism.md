# Concurrency Is Not Parallelism - Rob Pike

## Speaker

* [Rob Pike](https://en.wikipedia.org/wiki/Rob_Pike)
* [Twitter](https://twitter.com/rob_pike)

## Video

* [vimeo](https://vimeo.com/49718712)

<iframe src="https://player.vimeo.com/video/49718712?color=a086ee&title=0&byline=0&portrait=0" width="640" height="360" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>
<p><a href="https://vimeo.com/49718712">Rob Pike - &#039;Concurrency Is Not Parallelism&#039;</a> from <a href="https://vimeo.com/heroku">Heroku</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

## Slides

* [article](https://blog.golang.org/waza-talk)
* [slides](https://talks.golang.org/2012/waza.slide)

## Notes

* Go is a concurrent language.
* Concurrency is better than parallelism.
* **Concurrency** is the composition of independently executing things (functions or processes in the abstract).
* **Parallelism** is the simultaneous execution of multiple things (possibly related, possibly not)

* **Concurrency** is dealing with a lot of things at once.
* **Parallelism** is doing a lot of things at once.

* Concurrency can be used to run things in parallel, but concurrency is about structuring things.

* In a single-core computer you can have concurrency (and without that you would go mad), but you cannot have parallelism because at any given point in time there is only one thing that executes.

* [C. A. R. Hoare: Communicating Sequential Processes](https://www.cs.cmu.edu/~crary/819-f09/Hoare78.pdf)

* Concurrent composition of processes.

* Adding things to the design can make it more efficient.
* Parallelism can come from better concurrent expression of the problem.

