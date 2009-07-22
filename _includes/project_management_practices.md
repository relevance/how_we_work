## Project Management Practices {#project_management_practices}

Relevance uses a modified agile development methodology for ensuring development quality, timeliness and utility.
The components of our development strategy have been honed over years of experience;
however, our methods are flexible enough to suit the needs of a variety of different kinds of clients.
We will tailor our approach to each new project as necessary.

### Lifecycle

A development engagement with Relevance consists of a series of [iterations][],
and follows these general lifecycle stages:

* Iteration 0:
  An initial period of 2-10 days where the team establishes the development
  and testing environment, including project management and code repositories,
  staging services and databases, etc.
  Also, Business Analysis commences such that enough stories are in place
  to keep the development team busy for a full iteration.
* Iterations 1 - N:
  Development iterations, two weeks in length.
  At the beginning of each iteration we hold an iteration planning meeting
  to choose the highest priority functionality to be addressed.
  At the end of each iteration is a walkthrough of what was accomplished,
  as well as the delivery of a deployable application.  
* Final Iteration:
  Final wrap up of the functionality and deployment of the system
  to the production environment.
* Support Phase:
  Relevance works with the customer to deal with issues after the
  deployment of the application, addressing newly discovered defects or
  performance enhancements as needed.

### Communication

The most important part of any development process is the management of communication amongst the entire team, from developers to business analysts to beta customers and beyond.
We value communication above all else in our partnerships.
But communication doesn't just happen; therefore, we have many opportunities
for communication built into the structure of the project:

* daily standup meetings,
* iteration reports and iteration planning meetings,
* online discussion and commentary through the project wiki and story cards,
* periodic project retrospectives and risk assessments,
* and of course, emails and phone calls when things are unclear.

You will read more detail about all of those during the rest of this document.

### Project Tracking

We use [Mingle](http://mingle.thoughtworks.com) as our Project Management repository and living documentation source.
Requirements are documented as "User Stories" and represented
within the system as [cards][story_cards].
Each card has a title, a description, a detailed set of acceptance criteria, and an estimate of complexity.
Comments, changes, and research are all captured directly on the card.
As we proceed through iterations, cards are pulled in to the iteration as their priority dictates.

### Living Documentation

In addition to the story cards themselves, Mingle also provides a per-project [wiki](http://en.wikipedia.org/wiki/Wiki) where we keep documentation about architecture, system design, risk analysis, status reports, etc.
These documents comprise the system and process documentation for the entire project, and are viewable and editable by all members of the project team.

Here are the documents that are produced on a representative project, including evolving
documents maintained in Mingle as well as "point-in-time" documents that are usually
delivered via email:

Document                | Schedule                   | Author                    | Recipient   | Purpose
------------------------|----------------------------|---------------------------|-------------|--------
Story Cards             | Continuous                 | Entire team               | Entire team | Feature-level acceptance criteria and development status
Standup Report          | Daily                      | Relevance Project Manager | Entire team | Documentation of progress, blockers, new discussions
Iteration Status Report | Bi-weekly                  | Relevance Project Manager | Entire team | Stories accepted in previous iteration, major milestones reached
Risk Analysis Report    | Multi-iteration boundaries | Entire team               | Entire team | Documenting risks
Retrospective Notes     | Multi-iteration boundaries | Entire team               | Entire team | Process improvement
Wiki Documents          | Multi-iteration boundaries | Entire team               | Entire team | System design, architecture, general project knowledge
