### Quality Assurance (QA) {#qa}

Quality assurance is a transient role that developers assume as needed to
verify that a completed story meets its [objective acceptance criteria][]
before showcasing that story to stakeholders.

Most of our testing is fully automated, in the form of executable unit
tests or integration tests.
But automated tests can't catch every possible error.
The QA role should perform more "exploratory" testing, manually exercising
the feature and looking for problems (including problems with the user interface).
When possible, the developer in the QA role should identify additional automated tests
that would be helpful and either write such tests (if that can be done quickly,
as part of the QA process) or write a new story card for more involved tests,
so that they can be prioritized and scheduled by the customer.

The developer assuming the QA role should not be one of the same developers
who completed the story in question.
(Some simple stories can skip the QA step, not because there can't possibly be errors in them,
but because the likelihood is deemed small enough that the cost of QA would exceed the benefit.)
