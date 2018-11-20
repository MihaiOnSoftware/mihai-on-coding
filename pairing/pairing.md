# Pair Programming

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

## Addressing Pitfalls

The greatest pitfalls to pairing are:

* *Disengagement*
* *Watch the master*
* Communications breakdown
* Conflict

The first two can most often be resolved by switching the *driver* and *navigator* more often. Additionally by taking a more passive role in the *pair* and allowing the other *pairer* to take the lead. For some ways to facilitate this, take a look in the [Techniques](#Techniques) section, specifically [Ping-pong *Pairing*](#ping-pong-pairing) and [Pomodoro *Pairing*](#pomodoro-pairing).

For communications breakdown, where the *pairers* aren’t able to understand one another or feel unheard, taking a break from typing and having a discussion can help. One thing to try here is [Digging for Gold](#digging-for-gold), this often works very well to get the *pair* through a tough spot.

Conflict between the two *pairers* does happen sometimes. Addressing this is tricky and this doc won’t go into detail, but there are a lot of techniques on conflict resolution that can be helpful. There are quite a few [resources](http://sedano.org/toddsedano/2017/10/22/considerate-pair-programming.html) on pair programming specifically as well.

## *Pairing* *Station*


Before starting to *pair*, there should be a good space available that can facilitate and improve the *pairing* session. However, don’t let this be a barrier to pairing, if you can’t make/find a good space, ad-hoc over the shoulder pairing still works great! While having all of the criteria for the ideal *pairing* space is awesome, you’ll still get a lot of benefit even from pairing on a laptop at a table in the lunch area.

The ideal *pairing* *station* should meet the following criteria:

* Supports ease of screen reading for both *pairers*
* Makes it easy to switch the *driver* and *navigator*
* Makes it easy for both of the *pairers* to take the *driver*'s seat
* Isn't physically uncomfortable for either *pairer*
* Allows for direct communication
* Allows the *pairers* to communicate indirectly (e.g. visual cues)
* Includes a whiteboard for discussion
* In-person, though remote is possible if the environment can meet the above criteria.

### Screens

For in person *pairs*, having two monitors mirrored allows both *pairers* to see the work without looking over each other's shoulders.

For remote *pairs*, either screen sharing or live code sharing can work effectively. While live code sharing helps with switching, it makes it difficult to track non-code work.

### Switching

For in person *pairs*, having two keyboards and two mice works very well when combined with two mirrored monitors.

For remote *pairs* using some sort of live code sharing can make it simpler to switch *drivers*.

### Easy Driving

This is the hardest part.

For in person *pairs*:

* The keyboard(s) and mouse should be comfortable to use for both *pairers*. E.g.
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
* Both *pairers* should be able to sit comfortably while taking up either role
* Take into account all the normal considerations for comfort in the work place

For remote *pairs*:

* Both *pairers* need to be physically comfortable, can't have one (or both) member(s) in a cramped phone booth

### Direct Communication

The *pair* needs to be able to communicate directly, often verbally. If one or both of the *pairers* is a person with a disability that prevents verbal communication modify for other forms of communication. The goal is to be able to keep a constant dialogue going.

For in person *pairs*:

* The *pairers* need to be able to hear each other
* The work environment needs to allow for discussions and open communication, or the *pair* needs to have their own room

For remote *pairs*:

* Like in person, the *pairers* need to hear each other
* Both *pairers* need to be able to be loud enough to hear one another
* Both *pairers* need to easily hear/see the other *pairer*

### Indirect Communication

A large part of communication is not direct and triggered through subtle cues. If one or both of the *pairers* is visually impaired modify the recommendations for other indirect cues.

For in person *pairs*:

Able to see each other well enough to pick up on visual cues

For remote *pairs*:

* Both *pairers* need to be able to see each other while working, this can be tricky when sharing a screen.
* The *pairers* should be able to see each other's visual cues.

### Whiteboard

Having a whiteboard or some paper available for diagrams can help facilitate discussion immensely.

For in person *pairs*, an actual whiteboard or some paper works well.

For remote *pairs*, a piece of paper with the camera trained on it, or even better some virtual whiteboard.

## Roles

The two roles listed above, *driver* and *navigator* serve different purposes. It's often not clear who does what, keeping the guidelines here in mind can be helpful.

### *Driver*

This is the clearest role, at least in part, because it's the person at the keyboard. The *driver* is responsible for the implementation. They keep their focus on what is happening right now and interpret what the *navigator* is saying. It's best if the *driver* doesn't focus too much on the broader design. Instead they should focus on making sure the work they are doing right now is high quality and doesn't contain errors. For example while writing a method as directed by the *navigator*, the *driver* would focus on:

* extracting variables
* extracting private methods
* variable, method, and class names
* other local refactoring and improvements.

### *Navigator*

This role focuses on the broader scope of the *problem*. Generally the *navigator* will set the direction the code should go in. For example they might say something like "We need to add a private method to this class, something like `sanitize_svgs` which would take in an `svg` and return the sanitized verizon by calling out to the `SvgSanitizer`". The *driver* will then take this and put it into code, modifying it to keep the code clean and error free. The *navigator* is also responsible to keeping an eye out for any errors, typos, or refactoring opportunities that crop up and the *driver* misses. Though this is not their primary role it's still important.

The *navigator* should try to keep from grabbing the keyboard, even when the solution seems clear. If a solution can't be communicated clearly enough to the *driver* for implementation, it might not be all that clear of a solution. 

### Dialogue

It's important to note that the *driver* isn't just implementing what the *navigator* says, they are part of a dialogue. The idea here is that the *driver* brings in the "low level" perspective from the code that's in front of them and what will actually work here, the *navigator* brings in a more bird's eye view and tries to imagine how what is being written now will fit in with the greater design. By switching roles with some frequency, the *pair* can ensure that they have a good handle of both perspectives. 

## Techniques

There are different techniques that a *pair* can try when *pairing* to improve the experience or learn something new. Some of these techniques can work in tandem, others are mutually exclusive. Picking a technique depends on who the members of the *pair* are and how they work together

### Ping-pong *Pairing*

This is a *pairing* technique derived from TDD's `red`→ `green`→`refactor` loop. It works best if one or both of the *pairers* are familiar with TDD but can also be a learning opportunity in the *novice*-*novice* style. This technique is also useful when two *experts* are *pairing* or when dealing with a particularly challenging *problem*. Finally, this is a great way to learn or improve TDD skills.

#### How?

We'll call one *pairer* left and the other right.

The steps to this technique:

1. `Red` → left starts off driving by writing a breaking test, right talks them through what the test should test and makes sure they follow the [three rules of TDD](http://www.javiersaldana.com/tech/2014/11/26/refactoring-the-three-laws-of-tdd.html)
2. `Green` → right picks up the *driver*'s seat and writes the implementation the passes the test, left guides them through this and makes sure they follow the [three rules of TDD](http://www.javiersaldana.com/tech/2014/11/26/refactoring-the-three-laws-of-tdd.html)
3. `Refactor` → right continues in the *driver*'s seat and refactors both the production and test code, left keeps the broader picture in mind and guides the refactor 
4. The *pair* starts again but this time right is the *driver* and writes the test, they then switch so that left writes the implementation

### Pomodoro *Pairing*

This is a *pairing* technique based off of the [pomodoro technique](https://en.wikipedia.org/wiki/Pomodoro_Technique). This technique is helpful with resolving a *watch the master* situation or more generally in a *expert*-*novice* pair.

#### Pomodoro Technique?

This is a quick breakdown of the pomodoro technique, not pomodoro *pairing*.

1. Pick a task
2. Start a 25 min timer (this is a pomodoro)
3. Work until the timer rings or you've completed the given task
4. Take a 5 min break where you spend time not thinking about work (no emails!)
5. Repeat
6. After your fourth pomodoro take a 35 min break
7. Start again

This leads to ~2.5 hours per cycle. Along the way jot down the following:

* What task a given pomodoro is for
* "Hard" interruptions (anything that completely takes your attention away from the given task) usually denoted with a `-` on a piece of paper
* "Soft" interruptions (brief internal distractions) usually denoted with a `.` on a piece of paper

If there are enough interruptions, restart the pomodoro (usually without a break)

#### How?

We'll call one *pairer* left and the other right.

The steps to this technique:

1. Start a pomodoro
2. For this pomodoro left is the *driver* and right is the *navigator*
3. Take the 5 min break, step away from the *pair* and do something individually
4. Start another pomodoro
5. For this pomodoro right is the *driver* and left is the *navigator*

It's ok to sometimes switch roles within the pomodoro but each of the pariers should stick to the given role for the majority of the pomodoro. During the pomodoros keep track of the same things as a normal pomodoro.

After completing the *pairing* *session*, reflect on the number of distractions, what needs to improve?

### Digging for Gold

Sometimes one of the *pairers* will have a hard time listening the the other. They might feel that the other *pairer*'s ideas don't have merit or are lacking expertise. In these cases it's useful for the *pairer* that's having trouble finding value in the *pair* to try digging for gold. This technique is also useful when the *pair* is stuck and can't find a way forward.

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

### Starting Your *Session*

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

### On-boarding

Not a technique for pairing so much as a way to use it, having pairing as part of your on-boarding process will help in many ways:

* The on-boardee will learn what's needed quickly
* The *pair* will build a working relationship more quickly
* The on-boardee can start contributing right away
* Increases satisfaction at having joined the team

One interesting way to do this is to set up an [on-boarding sprint](http://blog.gdinwiddie.com/2013/03/27/adding-a-new-team-member/) for the on-boardee
