# Learning Software

## Books

When I recommend skimming, this usually means that you should come back to it at some point (maybe a long time from now, like a year or three) and give it another skim. Usually your experiences will help guide you to the information that's relevant to you.

### Refactoring by Martin Fowler

`Make the change easy, then make the easy change - Kent Beck`

This book is very valuable. It explains what code smells are, lists them out, and explains how to work with them. However this is not a "front to back" style read. I would recommend reading the chapters that describe what code smells are in general, what refactoring is in general, and then skim the different code smells with their related refactorings.

### Clean Code by Robert C. Martin

Another great book that can provide a lot. I would recommend reading the chapters that describe the SOLID principles and skimming the rest for what stands out. Specifically the SOLID principles are best read in the following order: SDOLI. This is not because some are more important than others, rather this is the order you are likely to come across them.

### Domain Driven Design by Eric J. Evans

This goes together very well with [Clean Code](#clean-code-by-robert-c-martin). I recommend reading the first few chapters completely and then skimming the rest. Domain driven design works really well together with the [clean or hexagonal architecture](http://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)

### Working Effectively with Legacy Code by Michael Feathers

This book is great for learning how to create and exploit what Feathers calls "seams". The reason these are useful is often we want to introduce some architectural change to the system, but it requires a massive refactor. Making use of this concept of "seams" allows one to introduce a change that gradually replaces the current system rather than having to do a big bang refactor.

### Design Patterns: Elements of Reusable Object-Oriented Software by the gang of four

Though this is a very valuable book, I highly recommend skimming it and only going into depth when needed. A great resource that contains much of the same information is available at [refactoring.guru](refactoring.guru).

### Refactoring to Patterns by Joshua Kerievsky

Another book that helps you make architectural changes to a system in a controlled and safe manner. It builds upon [Martin Fowler's Refactoring](#refactoring-by-martin-fowler) and [the gang of four's Design Patterns](#design-patterns-elements-of-reusable-object-oriented-software-by-the-gang-of-four) and links them together. It's useful to skim through this book and read a few examples in depth, it's also useful as a reference book when you've got a particular pattern in mind that you want to implement.

### Pragmatic Programmer by Andy Hunt and Dave Thomas

This is a classic, although parts of it are a little dated. This is a book that can be read start to finish unlike some of the others, however I suggested skipping the chapters on IDEs and metaprogramming (don't recall what they're called), these aren't as relevant today as they once were since the tools have changed tremendously. Metaprogramming specifically isn't great, as we've learned in the years since this book was written (a lot of companies used to have their own C macros that are completely unmaintainable garbage now).

### Extreme Programming Explained by Kent Beck

Talks about a lot of different practices of XP and the ideas behind them. This one can *mostly* be read front to back, but it can also be skimmed.

### Seven Languages in Seven Weeks by Bruce Tate && [exercism.io](exercism.io)

Learning another language can be very helpful as it helps give perspective on how different paradigms work. Often this helps you to bring in new ideas that are prevalent in another language or even to make small quality of life improvements in your code.

## Articles, videos, e.t.c.

### Martin Fowler
Martin's a very prolific author, I highly recommend reading pretty much everything on his blog. Some highlights:
* https://martinfowler.com/ieeeSoftware/yetOptimization.pdf
* https://www.martinfowler.com/bliki/CannotMeasureProductivity.html
* https://martinfowler.com/bliki/DesignStaminaHypothesis.html

But there's so much more...

### Michael Feathers
Feathers doesn't write that much in his blog, though if you have twitter he's worth a follow. However it's worth perusing what he has written, and some of his talks are really good (albeit a bit dry).
* https://michaelfeathers.typepad.com/michael_feathers_blog/2008/06/the-flawed-theo.html
* https://michaelfeathers.typepad.com/michael_feathers_blog/2013/11/unconditional-programming.html
* https://www.youtube.com/watch?v=AnZ0uTOerUI

### J. B. Rainsberger
Jbrains (as he calls himself) has some really good info on TDD especially.
* https://blog.thecodewhisperer.com/permalink/integrated-tests-are-a-scam
* https://blog.jbrains.ca/permalink/productivity-for-the-depressed

He has two blogs, which is annoying, but the content is pretty good.

### Robert C. Martin
Uncle Bob is hit and miss unfortunately. He has a lot of good stuff to say, but it's often obscured by his rather annoying personality. He has great resources on TDD and Clean Architecture. The Clean Coder videos are pretty good too, though you'll have to deal with his personality a lot.

### Kent Beck
When you can find talks or articles by him, they're always gold. Though they tend to be rare. Following Kent on twitter is worthwhile too.

### Michael D. Hill (aka GeePaw Hill)
Hill has a weird way of speaking and writing that can hurt the brain a little, however here are some of the more coherent tidbits:
* http://geepawhill.org/pro-tip-no-smaller/
* https://twitter.com/GeePawHill/status/1086748964936994816
* http://geepawhill.org/a-sense-of-urgency-ramps-as-a-motivation-model/

### Others
Here are some other things that I think are worthwhile reading/watching:
* https://xprogramming.com/classics/expemergentdesign/
* https://www.infoq.com/presentations/Simple-Made-Easy
* https://www.gamedev.net/blogs/entry/2265481-oop-is-dead-long-live-oop/
* http://www.ralin.net/blog/oop-anti-patterns-utility-or-helper-classes.html


