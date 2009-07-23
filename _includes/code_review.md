## Code Review {#code_review}

Our ideal mode of development is [pair programming][].
Sometimes, though, it's simply not practical to pair on every task.
Sickness, vacations, doctor appointments, and other things might interrupt a pair's work together.

At such times a task can be tackled by a solo developer.
But solo tasks must always be reviewed by another developer on the team.
(And the solo developer will try to choose a task that's relatively simple,
leaving the more complicated tasks for pair work.)

Our [task management system][story_cards] is configured to give a task two paths out of development.
The one we prefer is "Completed by Pair, Ready for QA."
But tasks handled by a solo developer follow an alternate path: "Completed Solo, Ready for Code Review."
That allows us to ensure that *every* piece of code that gets delivered to our customers has been seen by at least two developers.
Of course, that doesn't mean there aren't any problems, but it does shorten an important
[feedback loop][feedback_loops], catching most problems early, when fixing them is cheapest.
