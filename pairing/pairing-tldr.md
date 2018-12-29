# :pear:ing Cheat Sheet

## Why

Keep these in mind when pairing, use them to guide your pairing session and what you want to get from it.

* Remove knowledge silos to increase teams’ resiliency
* Build collective code ownership
* Improve learning
* Increase efficiency
* Improve software design
* Improve software quality
* Reduce the incidence of bugs
* Increase satisfaction
* Help with team building
* Faster on-boarding
* Serves as a short feedback loop, similar to a live code review
* Increases safety and trust
* Increases confidence

## Pitfalls

Watch out for these potential pitfalls, address them as soon as possible.

* Disengagement
* Watch the master
* Communications breakdown
* Conflict

## Station

The ideal pairing station should meet the following criteria:

* Supports ease of screen reading for both pairers
* Makes it easy to switch the driver and navigator
* Makes it easy for both of the pairers to take the driver's seat
* Isn't physically uncomfortable for either pairer
* Allows for direct communication
* Allows the pairers to communicate indirectly (e.g. visual cues)
* Includes a whiteboard for discussion
* In-person, though remote is possible if the environment can meet the above criteria.

Don't let this stop you from pairing though! These are aspirational goals.

## Roles

There a definitive roles in pairing, this doesn't mean that the roles don't intersect, rather that their focuses are different.

### Driver

The driver focuses on the immediate details in front of them, they are the ones doing the typing and making sure the code they're writing is clean. Don't start implementing your own strategy, if you have an idea stop and talk with your navigator.

The driver is responsible for:

* extracting variables
* extracting private methods
* variable, method, and class names
* other local refactoring and improvements
* method level design
* making sure that they understand what the navigator is saying
* bringing up concerns on the design with respect to implementation
* making moment to moment decisions on how to implement the strategy

### Navigator

The navigator focuses on the high level design and strategy, keep an eye out for bugs and typos, and be a reviewer of the code the driver is implementing. As a navigator you should keep your hands off the keyboard.

The navigator is responsible for:

* class level design
* structural level design
* keeping the problem at hand in mind
* guiding the driver in implementing the strategy
* making sure the pair stays on the problem and doesn't deviate too much
* ensuring learning goals are being met

## Techniques

For these techniques one pairer will be refered to as left, and another as right. When using this technique, try to be more strict as to the role division.

### Ping-pong *Pairing*

This technique is useful to ensure equal time driving/navigating and to learn TDD. It's great at resolving a watch the master situation

While following the [three rules of TDD](http://www.javiersaldana.com/tech/2014/11/26/refactoring-the-three-laws-of-tdd.html) and the `red`-->`green`-->`refactor` cycle, you can integrate pairing in the following way:

1. While writing a failing test (`red`): left drives, right navigates.
2. While writing the implementation to pass that test (`green`): right drives, left navigates.
3. While refactoring both the implementation and the test (`refactor`): right drives, left navigates.
4. Repeat, this time right drives during `red` and left during `green`/`refactor`

### Pomodoro *Pairing*

This is based off of the [pomodoro technique](https://en.wikipedia.org/wiki/Pomodoro_Technique). This technique is useful if you're having a hard time making sure you spend equal ammounts of time driving/navigating.

1. Start a 25 min timer, during this time left drives and right navigates.
2. After 25 min, take a 5 min break away from the pairing and your pair
3. Start another 25 min timer, during this time right drives and left navigates.
4. Take another 5 min break.
5. Repeat until you've completed 4 25 min blocks, switching driver and navigator every 25 min block
6. After 4 25 min blocks (and associated breaks), take a 35 min break or end the session.

Before each 25 min interval, note down what you're working on.
During each 25 min interval, note down any interruptions that break the flow.

### Digging for Gold

This technique is useful for unblocking yourselves or dealing with communications breakdown.

One of the pairers makes a naive or impractical suggestion for moving forward. The pair then takes this idea and looks for divergent ideas that could help solve the problem. The pair explores this solution, and divergent solutions, until they've either found one that works or feel they've found all the gold there is.

#### Tips

* "OK, how would that look in practice? We would need to..."
* "I think the problems with this approach are... maybe we can try... to address those"
* Try actually starting along that path
* If you end up in a rabbit hole, recall the problem you're trying to solve and bring the pair's attention back to it.

### Retrospective

Spend some time reflecting on the pairing session afterwards. Try to find areas of improvement on the way you pair. Potentially set a learning goal for next time and check-in to see if you've made progress toward that goal.

### Don't Rush

When one of the pairers moves forward too quickly, it's good for them to check in with their pair before forging ahead. Pairing requires that both members of the pair are on the same page and understand what's happening.