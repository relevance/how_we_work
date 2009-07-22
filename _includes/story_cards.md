### Story Cards {#story_cards}

Relevance manages requirements and tasks using *story cards*.
Story cards are a common feature of agile methods;
instead of a big requirements document in which small details can get lost,
each requirement or task has its own card, which records the task name, details (including acceptance criteria),
priority, estimate, and other information.

Cards don't have to be real, physical cards
(although on some large projects we've found it helpful to have a face-to-face meeting where
real cards are used).
We use a tool called [Mingle](http://studios.thoughtworks.com/mingle-agile-project-management)
to manage virtual cards and view them in various ways.

Cards have many advantages.
Cards push us toward very small granularity requirements, which improves estimates.
It's also easy to see what's been done and what's left if you track via cards.

Each card has a *status*, and moves through a lifecycle:

* Open
* Ready for Development
* In Development
* Ready for Code Review (if developed by a single programmer)
* Ready for QA
* Ready for Showcase
* Accepted

The client is responsible for two of those transitions.
The client must decide if the requirements are correct and move the card to
"Ready for Development".
Then, when the card is in the "Ready for Showcase" state,
the client is responsible for final testing and either marking the
card as "Accepted" or commenting on why it has not been accepted and moving it back
into "Ready for Development".
