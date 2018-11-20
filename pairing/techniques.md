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
