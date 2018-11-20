## Basics

Pair Programming is two people writing, debugging, or exploring code together. In essence it's simple, but getting the most out of your *pairing* *session* can take some work.

Pair programming is a complex practice requiring skill to master. There are a lot of resources on pair programming but some teams drop engineers into a *pair* expecting them to figure it out.

### Terminology

*Problem*: The work the *pair* is doing, what is being solved or explored.

*Pair* or :pear: : 

* (noun) Either the two people pair programming, or the *pairing* partner of the current subject. E.g. "The *pair* can try alternating roles", "Try spending some time asking your *pair* about their day before you start working on the *problem*".
* (verb) The act of pairing, e.g. "to pair or not to pair, that is the question"


*Pairer*: A member of a pair

*Session*: A stretch of time where two people are *pairing*. This ends when the *pair* splits up for anything more than a short break.

*Driver*: This is the *pairer* at the keyboard typing away. Despite what [NCIS](https://www.youtube.com/watch?v=msX4oAXpvUE) taught us, it's not actually useful or practical to have more than one person at the keyboard.

*Navigator*/*Observer*: This is the *pairer* that isn't currently *driving*. More details on this and the *driver* later. Generally, the *navigator* is responsible for reviewing the code the *driver* is writing, similarly to a code review.

*Development Environment*/*Station*: This is the environment in which the *pairing* is happening. Including: the desk, computer(s), keyboards, IDE. Anything that might improve or diminish the *pairing* *session* outside of the *pair* itself.

*Solution*: The approach currently taken to either resolve the *problem* or explore it.

*Expert*: The member of the *pair* that is relatively more experienced or knowledgeable. Especially in the particular *problem*. Not related to seniority and often isn't.

*Novice*: The member of the *pair* that is relatively less experienced or knowledgeable. Especially in the particular *problem*. Not directly related to seniority and often isn't.

*Disengagement*: When one member of the *pair* isn't focusing on the work being done or engaging in the *pairing*. This means that person is wasting their time. This is the biggest pitfall of *pairing*, as such it needs to be avoided or addressed.

*Watch the master*: Where an *expert* does performance programming while the *novice* watches and doesn't take part. This often lowers the satisfaction for the *novice* as well as misses out on the key contributions from the *novice*. This can also lead to *disengagement*, break down the *pairers'* relationship, and doesn't lead to learning. Not always a problem but it can be especially if repeated.

### But Why?

Aside from making work more enjoyable (though it may take some practice) there are some tangible benefits around the work itself. *Pairing* can:

* Remove knowledge silos to increase teams’ resiliency
* Build collective code ownership
* Improve learning
* Increase efficiency
* Improve software design
* Improve software quality
* Reduce the incidence of bugs
* Increase [satisfaction](http://sunnyday.mit.edu/16.355/williams.pdf)
* Help with team building
* Faster on-boarding
* Serves as a short feedback loop, similar to a live code review
* Increases safety and trust
* Increases confidence

### Types of pairs

#### *Expert*-*Expert*

If both parties are knowledgeable within the *problem* space.

Pros:

* Sharing of knowledge and ownership of the *solution* which increases team resiliency
* Reduce the incidence of bugs
* Greater satisfaction
* Both members of the *pair* can learn new things if they have different approaches
* Can improve software design and quality since the review feedback loop is short
* One or both of the *pairers* can introduce learning into the *session*.
* Helps with team building

Cons:

* Can create an echo chamber where the *pair* doesn't try new approaches
* Might resolve the *problem* faster, but at the cost of more total man-hours
* Can lead to *disengagement* if both *experts* take the same approach or the *problem* is simple

This works best if both members of the *pair* are *experts* in different parts of the *problem* space. E.g. One is an *expert* in the ins and outs of the area of code the *problem* is in, while the other is an *expert* in the *problem* type. In this case *expert*-*expert* *pairing* can be very effective.

#### *Expert*-*Novice*

The most traditional type of *pairing*, in broad terms this is the most beneficial in the most scenarios.

Pros: All the benefits of *pairing*. The *novice* brings insight and questions the status quo, the *expert* provides mentorship and can guide the flow.

Cons: Can lead to a "*watch the master*" scenario.

#### *Novice*-*Novice*

This type of *pairing* involves a lot of learning and discovery. Often happens when exploring a new area or working on something unusual. This type of *pair* has a lot of benefits, but also the most potential downsides.

Pros:

* Can be extremely satisfying
* Lots of learning involved
* Often leads to some interesting and unique *solutions*
* Improved code quality and incidence of bugs
* Great for team building
* Leads to collective code ownership
* Increases team resiliency

Cons:

* Can lead to introducing and reinforcing bad practices
* Can lead to the *pair* getting stuck and wasting time
* Can be very frustrating if the *pair* gets stuck

