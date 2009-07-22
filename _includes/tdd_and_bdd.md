## Test- and Behavior-Driven Development {#tdd_and_bdd}

### Test-Driven Development {#tdd}

At Relevance, we write most of our code in a "test-driven" style.
Test-driven development (TDD) means that, before writing a bit of production code that's required,
we'll first write an automated test that verifies that the code is working correctly.
(Which, of course, it isn't at the time we write the test, so the test fails.)
Then we'll go write the code that's necessary to make the test pass.
Lather, rinse, repeat.
That whole cycle often takes a minute or less.

TDD is incredibly valuable, for numerous reasons:

* As one of our employees has pointed out, it's possible to
  [fail even if your test suite seems thorough][failwith100].
  TDD is the best way we know to ensure that our tests actually cover all the *requirements*,
  not just all the *code*.
* TDD helps us focus on what the code needs to do, so we avoid the trap of building "nice to have"
  features that the customer doesn't value.
* TDD radically shortens the feedback loop between making a coding error and *discovering* that error.
  Debugging time is slashed by a huge amount.
  (Even if all of the other benefits did not exist, this alone would pay for the time spent writing tests.)
* The tests---especially if they're written in a very expressive style ([see below](#bdd))---serve
  as technical documentation about how the code should work.
  This documentation is very useful to future developers who might take up maintenance or further
  development on the project.
  And [continuous integration][] ensures that these tests always reflect
  the actual state of the system, which makes them far superior to a prose design document.
  (We've never seen one of those that wasn't very outdated.)
* Code that's really well designed is also very testable.
  In fact, one of the best ways to ensure that your code is well designed is to require that
  it be testable.
  (And the best way to do that is to build it through testing!)
  TDD helps us deliver code that has high cohesion and loose coupling, and a lot of other
  qualities that may seem like just so much programmery jargon, but which do make the
  systems less costly to maintain and enhance over time.
  
### Behavior-Driven Development {#bdd}

"Behavior-Driven Development" (BDD) is a style of test-driven development that focuses on
a different way of *expressing* the tests, using different terminology that emphasizes
the test's role as *specification*.
For example, in BDD, we try to refrain from calling
them "tests," even though testing remains a big part of the purpose.
Instead, they are called "specs" or "examples," to remind us of the many ways they support the project
beyond just "testing."

BDD doesn't add anything new *technically* beyond TDD;
rather, it's a shift in focus, seeing the specs not merely as error-detection tools
but as communication tools, helping us to better understand requirements
(and to *know* that we've understood them) and to record them in a useful way.
BDD also emphasizes specs that focus on externally visible behavior of the system
or component, rather than focusing on internal state.
That shift highlights the role of BDD as a design tool.

The tools we use for BDD mean that, in many cases, specs and examples can be read and understood
by customer representatives, including domain experts (perhaps with a little help from us).
That's really valuable, especially when the requirements are tricky, because it helps us to
be clear and precise, and to know that we're really building what our customers want.