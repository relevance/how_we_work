## Interpreting the Agile Manifesto {#agile_manifesto}

The Agile Manifesto provides very broad guidelines:

> We are uncovering better ways of developing
> software by doing it and helping others do it.
> Through this work we have come to value:
> 
> * Individuals and interactions over processes and tools
> * Working software over comprehensive documentation
> * Customer collaboration over contract negotiation
> * Responding to change over following a plan  
> 
> That is, while there is value in the items on
> the right, we value the items on the left more.
> 
> --[Agile Manifesto](http://agilemanifesto.org/)
> {: .attribution}

First of all, _don't stop reading after the list!_
The things on the right do have value.
The manifesto is about what gets _priority_, not what gets _done_.

That said, here's how we put these guidelines into practice:

### Individuals and Interactions {#individuals_and_interactions}

The first principle of the Agile Manifesto is to value individuals and interactions over processes and tools.

As software developers, we are actually passionate about tools.
And we love our processes as well.
Both processes and tools help us get things done.

But tools and processes can't get in the way of people and relationships.
This principle guides us in choosing tools.
We choose tools that amplify the individual's effectiveness, rather than tools that the person has to steer and control.
And we choose tools that facilitate collaboration and communication.
Here is a short list of examples:

* Ruby and Clojure, our preferred programming languages, have a lot of power and allow programmers to be expressive and clear, without a lot of ceremony that must be observed.
* Rails, our preferred web development platform, solves the most common and well-understood problems of web development for us, but gets out of our way when we need to do something unusual.
* The Git source control system (along with GitHub, the Git-based central repository we use) is designed to facilitate collaboration and experimentation.
  It also makes switching between tasks very fast and cheap.
* RSpec (including our own variant of it, Micronaut) allows us to write clean, expressive executable tests that serve as documentation of how the code should work.
* Our office workspace is designed around pairing stations.
  They allow two programmers to work together easily on the same problem.

In addition to tools, we choose processes that emphasize people and communication.
Pair programming is a part of that, and so is the daily standup meeting.
We have retrospectives to talk about what went well and what could be improved
(and usually people, not tools, are at the core of both of those topics).

### Working Software {#working_software}

The second principle of the Agile Manifesto is to value working software over comprehensive documentation.

At Relevance, we keep software working and ready to ship throughout the development lifecycle by:

* regular deployment to the [staging environment][staging]
* [TDD and BDD][]
* [continuous integration][]
* [pair programming][]
* [code review][]
* [iterations][]

It's also important to discuss documentation.
Historically, in software development, it's been a priority to exhaustively document everything:
requirements, design, test suites, correct usage, and so on.
But that's expensive; so expensive that often the software itself suffers from the effort devoted to documentation.
So we don't write documentation _just because_; we write documentation when it has value.
(And we work with our customers to decide whether it's valuable to them.)
Also, we try to write documentation that pays for itself in more than one way.

Occasionally, our customers will want traditional documentation:
prose descriptions of architecture, design, or correct usage, with diagrams.
We'll happily do that!
It becomes a task which is scheduled along with the developement tasks, and its priority (as with all tasks) is determined by the customer.

More often, though, that kind of documentation just isn't a high priority.
There are two kinds of documentation that are always really important, though.
They are:

* documentation that helps users understand how to use the software
* documentation that helps future programmers (maybe even us!) understand how to fix, maintain, and extend the software.

These days, the first problem is usually tackled simply by making the system more _usable._
When is the last time you read a user manual for a piece of software?

The second problem we solve through tests---executable specifications for how the system (in whole or in part) should work.
The tools we use allow us to write specs that read like design documentation to skilled programmers,
and some of our specs can be understood and verified by our customers.
Both of these techniques have two important advantages over traditional design documentation.
First, because they can be used to find errors in the system, they don't cost any extra; they're a part of the development and QA processes.
Second, as long as we insist that those test all run successfully (via [CI][continuous_integration]), we know that they aren't out of date---they still reflect the way the code actually works.

### Customer Collaboration {#customer_collaboration}

The third principle of the Agile Manifesto,
valuing "customer collaboration over contract negotiation",
can seem self-serving when it's a vendor saying the words.
But of course, as many customers have learned, contracts can be exploited by _both_ sides, as both shields and weapons.
(We've heard other developers say "They're going to hate it, but we're giving them exactly what the contract specifies.")

Contracts are important and useful, and time spent negotiating them can be well spent.
But when that gets in the way of effective collaboration, it's a bad trade.
Customer/vendor relationships are much better when the two are working together as partners,
and when the sense of safety is built into the way you work.

{% comment %}
I think the point I'm trying to make in the next paragraph is the right one---
that we try to build the things others use contracts for (incentives, controls, and defense)
into the way we work rather than into the contract---
is the point we want to make.
But I'm not at all happy with the way it's expressed right now.
(Glenn)
{% endcomment %}

Here's just one example out of many:
One of the many reasons we like to work in [iterations][iterations] is that we can deliver working software to the customer every other week.
That means if there's some external reason (like a sudden budget crunch) that they need to cut the project short, they will have still received something valuable from the relationship.
And we like to educate our customers about our standards (this website is part of that effort) so that they can see how we work, and hold us to our promises if necessary.
GitHub allows our customers to look at the code if they are interested, and especially the specs.
RunCodeRun allows them to watch our test suite grow, and see that we are keeping the tests passing.

### Responding to Change {#responding_to_change}

The fourth principle of the Agile Manifesto is to value responding to change over following a plan.

At Relevance, the following practices help teams respond quickly to change:

* the [daily standup][]
* the [story card lifecycle][story_cards]

The principle doesn't devalue *planning*---just sticking to the plan.
Planning is valuable in itself, and because the plan helps us recognize when things have changed;
it helps us understand the implications of change, how we need to adjust, and the likely cost.
The important thing is that, as we make plans, we understand that the plan may have to change.
Planning is an ongoing timeboxed activity that includes

* [iteration planning meetings][iteration_planning]
* [retrospectives][]
* [risk assessments][]
