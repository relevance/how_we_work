### Technical Debt

We like to use the metaphor of "technical debt" to describe parts of a
system's code that isn't as cleanly written or well designed as it should be.

Like all metaphors, the technical debt metaphor breaks down if you stretch it too far,
but it's a good way to think about the impact of design or development "short cuts."

* Like real debt, sometimes it is useful for taking advantage of opportunities now,
  rather than later.
* Like real debt, if you don't carefully manage it and pay it down,
  it becomes a drain on your resources
  (in this case, your development resources and productivity).
* Like real debt, technical debt is easy to ignore if you don't focus on it from
  from time to time.

As customers and users, you don't see technical debt directly.
But you do see its effects.
Users see technical debt in persistent bugs, or in new bugs that pop up when old ones are fixed.
And customers see it in declining productivity over the life of the project.
(Have you ever wondered why small enhancements to old software seem to take
almost as long as it took to write all of version 1?)

We regularly discuss the technical debt on our projects, and keep track of it.
Then, when we're visiting that area of the code again for other purposes, we choose
to clean it up rather than continuing to pay interest in the form of lost productivity.

This is an ongoing audit of the internal quality of the system.
It's usually less visible to stakeholders than the other audits,
but we will keep the customer aware of our activities related to technical debt.
