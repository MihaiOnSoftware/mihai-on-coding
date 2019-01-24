# Pair programming explained

## TL;DR

Pair Programming is two people writing, debugging, or exploring code together. In essence it's simple, but getting the most out of your *pairing* *session* can take some work.

Pair programming is a complex practice requiring skill to master. There are a lot of resources on pair programming but sometimes engineers are dropped into a *pair* with little preparation are expected to just figure it out.

## Table of contents
* [What, when, why, and who](#what-when-why-and-who)
* [Roles](#roles)
* [Addressing pitfalls](#addressing-pitfalls)
* [*Pairing* *station*](#-pairing-station)
* [Techniques](#techniques)
* [Other resources](#other-resources)

## What, when, why, and who

### Terminology (What?)

*Problem*: The work the *pair* is doing, what is being solved or explored.

*Pair* or :pear:: 
* (noun) Either the two people pair programming, or the *pairing* partner of the current subject. E.g. "The *pair* can try alternating roles", "Try spending some time asking your *pair* about their day before you start working on the *problem*".
* (verb) The act of pairing, for example "to pair or not to pair, that is the question".

*Pairer*: A member of a pair.

*Session*: A stretch of time where two people are *pairing*. This ends when the *pair* splits up for anything more than a short break.

*Driver*: This is the *pairer* at the keyboard typing away. Despite what [NCIS](https://www.youtube.com/watch?v=msX4oAXpvUE) taught us, it's not actually useful or practical to have more than one person typing at the same time.

*Navigator*: Sometimes called the *observer* (though this is inaccurate). This is the *pairer* that isn't currently *driving*. More details on this and the *driver* later. Generally, the *navigator* figures out the strategy, and guides the *driver* in implementing that strategy.

*Development Environment*/*Station*: This is the environment in which the *pairing* is happening. Including: the desk, computer(s), keyboards, IDE. Anything that might make the *pairing* *session* better or worse outside of the *pair* itself.

*Solution*: The approach currently taken to either resolve the *problem* or explore it.

*Expert*: The member of the *pair* that is relatively more experienced or knowledgeable. Especially in the particular *problem*. Not related to seniority and often isn't.

*Novice*: The member of the *pair* that is relatively less experienced or knowledgeable. Especially in the particular *problem*. Not directly related to seniority and often isn't.

*Disengagement*: When one member of the *pair* isn't focusing on the work being done or engaging in the *pairing*. This means that person is wasting their time. This is the biggest pitfall of *pairing*, as such it needs to be avoided or addressed.

*Watch the master*: Where an *expert* does performance programming while the *novice* watches and doesn't take part. This often lowers the satisfaction for the *novice* as well as misses out on the key contributions from the *novice*. This can also lead to *disengagement* and break down the *pairers'* relationship. Sometimes *watch the master* is a valid mentoring approach, but it is not *pairing*.

### When?

Whenever! Pairing doesn't need to be structured or planned. Ad hoc *pairing* works very effectively, especially if the *pairers* have done a few sessions together already. This isn't to say that *pair*ing should be done constantly or in every circumstance, it's an individual decision. While there are some companies that do full time *pair*ing all the time, that's not for everyone.

It's important to keep in mind that *pair*ing is also quite tiring. While *pair*ing, the *pair* is always on the ball and focused, keeping that kind of long term focus can be exhausting. As such it's great to take some breaks, at least every 2 hours or so but whatever works. Additionally, just because one *pairer* is up to keep going, doesn't mean the other has to be.

### But why?

It’s important to understand why we *pair* and what we’re hoping to accomplish. This section isn’t definitive and can vary subjectively. Use these as  goals or areas where your pairing might improve.

Aside from often making work more enjoyable (though it may take some practice) there are some tangible benefits around the work itself. *Pairing* can:

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

### Who?

This is a somewhat shallow and brief breakdown, but it’s a good place to start. A more in-depth view makes use of the [Dreyfus Squared](https://cdn-images-1.medium.com/max/1600/1*jOo1uFxJ492652tC3H78cw.png) model. More can be found on this in [Patterns of Effective Teams by Dan North](https://www.youtube.com/watch?v=lvs7VEsQzKY) and in this [Software Engineering Wisdom blog post](https://ykode.id/software-engineering-wisdom-9fa1b27a826d).

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

* Can create an echo chamber where the *pair* doesn't try new approaches and lacks diversity of thought
* Might resolve the *problem* faster, but at the cost of more total man-hours
* Can lead to *disengagement* if both *experts* take the same approach or the *problem* is simple

This works best if both members of the *pair* are *experts* in different parts of the *problem* space. E.g. One is an *expert* in the ins and outs of the area of code the *problem* is in, while the other is an *expert* in the *problem* type. In this case *expert*-*expert* *pairing* can be very effective.

#### *Expert*-*Novice*

The most traditional type of *pairing*, in broad terms this is the most beneficial in the greatest number of scenarios.

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
	* These can be things that affect the final artifact directly (e.g. bad design) which can be mitigated by code reviews.
	* Or things that affect the process of producing the artifact (e.g. big design up front) which are difficult to mitigate
* Can lead to the *pair* getting stuck and wasting time
* Can be very frustrating if the *pair* gets stuck

## Roles

The two roles listed above, *driver* and *navigator* serve different purposes. It's often not clear who does what, keeping the guidelines here in mind can be helpful.

### *Driver*

This is the clearest role, at least in part, because it's the person at the keyboard. The *driver* is responsible for the implementation. They keep their focus on what is happening right now and interpret what the *navigator* is saying. It's best if the *driver* doesn't focus too much on the broader design. Instead they should focus on making sure the work they are doing right now is high quality and error free. For example, while creating a new class as directed by the *navigator*, the *driver* would focus on:

* extracting variables
* extracting private methods
* variable, method, and class names
* other local refactoring and improvements.
* method level logic
* private methods
* code style
* running the tests

### *Navigator*

This role focuses on the broader scope of the *problem*. Generally the *navigator* will set the direction the code should go in. For example they might say something like "Maybe we can pull these shared methods into another class and pass it into the constructors". The *driver* will then take this and put it into code, modifying it to keep the code clean and error free. Along the way, the *navigator* is responsible for keeping the *pairing* on track. They ensure that rabbit holes are stepped out of in a reasonable time and new approaches are tried as old ones fail to pan out. The *navigator* is also keeps an eye out for any errors, typos, or refactoring opportunities that crop up and the *driver* misses. Though this is not their primary role it's still important.

### Dialogue

It's important to note that the *driver* isn't just implementing what the *navigator* says, they are part of a dialogue. The idea here is that the *driver* brings in the "low level" perspective from the code that's in front of them and what will actually work here. Compared to the *navigator*, who brings in a more bird's eye view and tries to imagine how what is being written now will fit in with the greater design. By switching roles with some frequency, the *pair* can ensure that they have a good handle of both perspectives.

### Switching roles

Switching roles while *pairing* is essential to the process, it’s also one of the trickiest things to do correctly. The two roles have very different frames of reference. Switching roles is a pretty big context switch when the roles are followed effectively. As such there needs to be some care involved.

#### The wrong way

*Pairing* is about working together. Anything that impedes one of the *pairers* from contributing or breaks their flow is bad. Two of the more obvious ways to do this are to "grab the keyboard" or "push the keyboard".

Grabbing the keyboard: Sometimes when working as the *navigator* it's oh so tempting to just take the keyboard control away to quickly do something. This puts the current *driver* in a bad position. Not only are they now not contributing, but such a forceful role change is likely to lead to conflict.

Pushing the keyboard: Other times, the *driver* feels a strong need to direct the strategy. It's very tempting to just "push" the keyboard to the *navigator*, forcing them to take the *driver*'s seat, and start telling them what to do. This sudden context switch can be jarring and confusing to the unsuspecting *navigator*. It can lead to resentment and conflict as the *navigator* feels invalidated or ignored.

Finally even a consensual role switch can be jarring and confusing if done too quickly and without structure.

#### The right way

The first step to switching roles is always to ask. The *navigator* needs to ask if they can grab the keyboard before doing so. The *driver* needs to ask if the *navigator* is willing to drive before starting to direct them. Sometimes, switching without asking works out. These situations are the exception and asking **always** helps.

It's important to take some time when switching as well. Both *pairers* need to take some time acclimatizing to their new roles. This time can be reduced somewhat by having a structure around switching (e.g. [Ping-pong *Pairing*](#ping-pong-pairing)) . This allows the *pairers* to be mentally prepared for the switch to happen.

## Addressing pitfalls

The greatest pitfalls to pairing are:

* *Disengagement*
* *Watch the master*
* Communication breakdown
* Conflict
The first two can most often be resolved by [switching](#switching) the *driver* and *navigator* more often. Additionally by taking a more passive role in the *pair* and allowing the other *pairer* to take the lead. For some ways to facilitate this, take a look in the [Techniques](#Techniques) section, specifically [Ping-pong *pairing*](#ping-pong-pairing) and [Pomodoro *pairing*](#pomodoro-pairing).

For communication breakdown, where the *pairers* aren’t able to understand one another or feel unheard, taking a break from typing and having a discussion can help. One thing to try here is [Digging for gold](#digging-for-gold), this often works very well to get the *pair* through a tough spot.

Conflict between the two *pairers* does happen sometimes. Addressing this is tricky and this doc won’t go into detail, but there are a lot of techniques on conflict resolution that can be helpful. There are quite a few [resources](http://sedano.org/toddsedano/2017/10/22/considerate-pair-programming.html) on pair programming specifically as well.

### *Pair*ing misconceptions

Here's a brief overview of some pairing misconceptions. Another good resource is [Martin Fowler's blog post](https://www.martinfowler.com/bliki/PairProgrammingMisconceptions.html) on the topic.

#### Don't *pair* on rote code, only complex

One of the things that *pair* programming is great at is identifying code smells and opportunities for abstraction. Rote code is often a good source of both of these so *pair*ing can be very effective here

#### *Pair*ing is less productive

As Fowler points out in his [blog post](https://www.martinfowler.com/bliki/PairProgrammingMisconceptions.html), pairing is meant to help with the hardest parts of programming. The entire purpose is to be more productive.

#### But I don't like *pair*ing

Maybe that's true. Possibly it's a matter of lack of familiarity. If you've tried pairing and found that it didn't work, try a different partner, this makes a huge difference. If you feel lost or it's still not working, try some of the techniques near the end of this doc.

## *Pairing* *station*

Before starting to *pair*, there should be a good space available that can facilitate and improve the *pairing* session.

The ideal *pairing* *station* should meet the following criteria:

* Supports ease of screen reading for both *pairers*
* Makes it easy to switch the *driver* and *navigator*
* Makes it easy for both of the *pairers* to take the *driver*'s seat
* Isn't physically uncomfortable for either *pairer*
* Allows for direct communication
* Allows the *pairers* to communicate indirectly (e.g. visual cues)
* Includes a whiteboard for discussion
* In-person, though remote is possible if the environment can meet the above criteria.

### Bad stations are OK

Don’t let your environment be a barrier to pairing, if you can’t make/find a good space, ad-hoc over the shoulder pairing still works great! While meeting this criteria for the ideal *pairing* space is awesome, you’ll still get a lot of benefit even from pairing on a laptop at a table in the lunch area. If you find that pairing isn’t working for you, try some of the suggestions below as the station can help with a lot of problems.

### Screens

For in person *pairs*, having two monitors mirrored allows both *pairers* to see the work without looking over each other's shoulders. For Mac users, remember to bring that USB adapter!

For remote *pairs*, either screen sharing or live code sharing can work effectively. While live code sharing helps with switching, it makes it difficult to track non-code work.

### Switching

For in person *pairs*, having two keyboards and two mice works very well when combined with two mirrored monitors.

For remote *pairs* using some sort of live code sharing can make it simpler to switch *drivers*.

### Easy driving

This is the hardest part.

For in person *pairs*:

* The keyboard(s) and mouse should be comfortable to use for both *pairers*.
	* If one member uses left handed mice, the mouse they are using should work for them
	* The keyboards should be in a layout that is familiar to the *pair* using it
* Shortcuts and productivity commands should be comfortable for both *pairers*
	* The IDE plays a big part in this. E.g.
		* RubyMine/Atom/VSCode shortcuts and plugins
		* Vim commands and plugins
		* RubyMine/Atom/VSCode Vim integration can simplify switching when one member uses Vim and another uses an IDE
		* The command lookup shortcut can help
			* `CMD + SHIFT + A` for RubyMine
	* The OS and apps installed can also play a part
		* What type of shell
		* SequelPro vs mysql
		* Debugging tools
		* Postman
		* Browser

#### IDEs

These are a constant problem and can cause a lot of tension for the *pair*. The machine being used should **always** be able to accommodate the lowest common denominator. As an example, I’m not proficient in Emacs and only a little capable with Vim. If asked to pair on a machine with Emacs/Vim I would struggle to *drive*. Many modern IDEs like RubyMine, VSCode, Atom, etc. are much simpler to use and have a lower bar for entry. They also generally have Vim plugins, can quickly switch configurations, and have functionality lookups. It’s OK to switch IDEs when the driver switches, but less than ideal as switching is less fluid. Bottom line is: make sure the machine being *paired* on can support both *pairers*.

Any time a *pairer* ends up driving out of necessity check that it isn't because of the environment.

For remote *pairs*:

* Same as in person
* Having the environment local to one *pairer* can make it harder for both to drive
* Connectivity problems
* Switching delays
* Lack of access to shared resources

### Physically comfortable

The area both *pairers* are working in should be comfortable.

For in person *pairs*:

* Both *pairers* should have the same amount of physical space, especially when driving
	* [Curved corner desks](https://www.ikea.com/ca/en/catalog/products/S19282844/) can create a situation where one person is uncomfortably situated or has less space available to them.
* Both *pairers* should be able to sit comfortably while taking up either role
	* A small desk that’s enough for one person is usually uncomfortable for two people to sit at
* Take into account all the normal considerations for comfort in the workplace

For remote *pairs*:

* Both *pairers* need to be physically comfortable, can't have one (or both) member(s) in a cramped phone booth

### Direct communication

The *pair* needs to be able to communicate directly, often verbally. If one or both of the *pairers* is a person with a disability that prevents verbal communication modify for other forms of communication. The goal is to be able to keep a constant dialogue going.

#### I don’t like talking

It can be intimidating to think that you’ll be having a constant dialogue with someone. There are ways to make it easier to do while pairing. The first is the structure of pairing itself, the roles help smooth communication between individuals. When taking on a role there are guidelines on what to talk about and when. The second is trying some of the [techniques](#techniques) that are useful for pairing. These give you frameworks on when to switch roles, what kind of questions to ask, and even how to get over communication blockages.

#### Language barriers

Sometimes, the *pairers* don’t natively speak the same language. This is a pretty significant barrier to pairing and can cause some people to shy away from pairing. Whenever you feel that your pair hasn’t understood you, don’t forge on ahead. Spend some time clarifying what they’ve understood and defining things they don’t understand. Not only will this improve your pairing but it can help strength language skills in both *pairers*!

For in person *pairs*:

* The *pairers* need to be able to hear each other
* The work environment needs to allow for discussions and open communication, or the *pair* needs to have their own room

For remote *pairs*:

* Like in person, the *pairers* need to hear each other
* Both *pairers* need to be able to be loud enough to hear one another
* Both *pairers* need to easily hear/see the other *pairer*

### Indirect communication

A large part of communication is not direct and triggered through subtle cues. If one or both of the *pairers* is visually impaired modify the recommendations for other indirect cues.

For in person *pairs*:

Able to see each other well enough to pick up on visual cues

For remote *pairs*:

* Both *pairers* need to be able to see each other while working, this can be tricky when sharing a screen.
* The *pairers* should be able to see each other's visual cues.

### Whiteboard

Having a whiteboard or some paper to draw on can help facilitate discussion immensely.

For in person *pairs*, an actual whiteboard or some paper works well.

For remote *pairs*, a piece of paper with the camera trained on it, or even better some virtual whiteboard.

## Techniques

There are different techniques that a *pair* can try when *pairing* to improve the experience or learn something new. Some of these techniques can work in tandem, others are mutually exclusive. Picking a technique depends on who the members of the *pair* are and how they work together

### Ping-pong *pairing*

This is a *pairing* technique derived from Test Driven Development's (TDD) `red`→ `green`→`refactor` loop. It works best if one or both of the *pairers* are familiar with TDD but can also be a learning opportunity in the *novice*-*novice* style. This technique is also useful when two *experts* are *pairing* or when dealing with a particularly challenging *problem*. Finally, this is a great way to learn or improve TDD skills.

#### How?

We'll call one *pairer* **left** and the other **right**.

The steps to this technique:

1. `Red` → **left** starts off driving by writing a breaking test, **right** talks them through what the test should test and makes sure they follow the [three rules of TDD](http://www.javiersaldana.com/tech/2014/11/26/refactoring-the-three-laws-of-tdd.html)
2. `Green` → **right** picks up the *driver*'s seat and writes the implementation that passes the test, **left** guides them through this and makes sure they follow the [three rules of TDD](http://www.javiersaldana.com/tech/2014/11/26/refactoring-the-three-laws-of-tdd.html)
3. `Refactor` → **right** continues in the *driver*'s seat and refactors both the production and test code, **left** keeps the broader picture in mind and guides the refactor 
4. The *pair* starts again but this time **right** is the *driver* and writes the test, they then switch so that **left** writes the implementation

### Pomodoro *pairing*

This is a *pairing* technique based off of the [pomodoro technique](https://en.wikipedia.org/wiki/Pomodoro_Technique). This technique is helpful with resolving a *watch the master* situation or more generally in a *expert*-*novice* pair.

#### Pomodoro technique?

This is a quick breakdown of the pomodoro technique, not pomodoro *pairing*.

1. Pick a task
2. Start a 25 min timer (this is a pomodoro)
3. Work until the timer rings or you've completed the given task
4. Take a 5 min break where you spend time not thinking about work (no emails or slack!)
5. Repeat
6. After your fourth pomodoro take a 35 min break
7. Start again

This leads to ~2.5 hours per cycle. Along the way jot down the following:

* What task a given pomodoro is for
* "Hard" interruptions (anything that completely takes your attention away from the given task) usually denoted with a `-` on a piece of paper
* "Soft" interruptions (brief internal distractions) usually denoted with a `.` on a piece of paper

If there are enough interruptions, restart the pomodoro (usually without a break)

#### How?

We'll call one *pairer* **left** and the other **right**.

The steps to this technique:

1. Start a pomodoro
2. For this pomodoro **left** is the *driver* and **right** is the *navigator*
3. Take the 5 min break, step away from the *pair* and do something individually
4. Start another pomodoro
5. For this pomodoro **right** is the *driver* and **left** is the *navigator*

It's ok to sometimes switch roles within the pomodoro but each of the pairers should stick to the given role for the majority of the pomodoro. During the pomodoros keep track of the same things as a normal pomodoro.

After completing the *pairing* *session*, reflect on the number of distractions, what needs to improve?

### [Strong style](http://llewellynfalco.blogspot.com/2014/06/llewellyns-strong-style-pairing.html)

`For an idea to go from your head into the computer it *must* go through someone else's hands`

In this technique, the *navigator* has some idea how they want the *solution* to look. The *driver* drives as described in [*roles*](#Roles). Any time the *driver* has an idea they want to try out, the roles switch.


### Digging for gold

Sometimes one of the *pairers* will have a hard time listening to the other. They might feel that the other *pairer*'s ideas don't have merit or are lacking expertise. In these cases it's useful for the *pairer* that's having trouble finding value in the *pair* to try digging for gold. This technique is also useful when the *pair* is stuck and can't find a way forward.

#### How?

One of the *pairers* makes a naive or impractical suggestion for moving forward. The *pair* then takes this idea and looks for divergent ideas that could help solve the *problem*. The *pair* explores this *solution*, and divergent *solutions*, until they've either found one that works or feel they've found all the gold there is.

#### Tips

* "OK, how would that look in practice? We would need to..."
* "I think the problems with this approach are... maybe we can try... to address those"
* Try actually starting along that path
* If you end up in a rabbit hole, recall the *problem* you're trying to solve and bring the pair's attention back to it.

### Retrospective

Spend some time reflecting on the *pairing* *session*.

#### Tips

* "Do you feel that this was a balanced *pairing* *session*?"
* "How can we improve our *station*?"
* "How do you feel after our *session*?"
* “What did you learn/teach during our session?”
* “How do you feel about the progress we made?”
* “How did you feel about the length of the session?”
* “Is there anything that stood out to you during our pairing?”
* Set a learning goal for next time, reflect on this *session*'s learning goals

### Starting Your *session*

Spend some time before *pairing* talking about things not related to the *problem* at hand. This can set the tone for the *session* and make everyone feel comfortable.

#### Tips

* "How's it going?"
* "How was your weekend?"
* "What are you working on lately?"
* "Did you see the Packers' game last night?"

### Don't Rush

When one of the *pairers* moves forward too quickly, it's good for them to check in with their *pair* before forging ahead. *Pairing* requires that both members of the *pair* are on the same page and understand what's happening.

#### Tips

* "Do you know where I'm going with this?"
* "What do you think of moving along with this *solution*"
* Step back and don't write code for a while, discuss what you'll be doing instead.
* Don’t "just try this one thing" before explaining what you’re doing

### Rubber ducking

Though not a pairing technique, in the absence of a second person to pair with this can provide a (very) small part of the benefits of pairing. This is a solo exercise meant to help clarify thoughts. It's quite effective a sussing out hidden complexity in a given *solution* or alternate perspectives on a given *problem*.

#### How?

Take some inanimate object. In an ideal world this object is something the bobs gently on it's own like one of those solar powered flower toys or a rubber ducky floating in water, but anything that can be anthropomorphized works. Then explain, out loud, to the "rubber duck" what the *problem* is and what *solutions* present themselves. The process of explaining it in a way that a rubber duck would understand helps explore *problem* or the *solutions*.

#### This sounds dumb

It does, but it can be surprisingly useful.

### On-boarding

Not a technique for pairing so much as a way to use it, having pairing as part of your on-boarding process will help in many ways:

* The on-boardee will learn what's needed quickly
* The *pair* will build a working relationship more quickly
* The on-boardee can start contributing right away
* Increases satisfaction at having joined the team

One interesting way to do this is to set up an [on-boarding sprint](http://blog.gdinwiddie.com/2013/03/27/adding-a-new-team-member/) for the on-boardee

## Other resources

Here are some other great resources!

* http://sedano.org/toddsedano/2017/10/24/considerate-pair-programming.html
* https://codeburst.io/pair-programming-for-introverts-dab230879c84
* https://tuple.app/
* http://llewellynfalco.blogspot.com/2014/06/llewellyns-strong-style-pairing.html
* https://ykode.id/software-engineering-wisdom-9fa1b27a826d
* https://www.martinfowler.com/bliki/PairProgrammingMisconceptions.htm
