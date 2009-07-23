### Objective Acceptance Criteria {#objective_acceptance_criteria}

If you don't know what you are building, you won't know when you are done---and you will almost certainly build the wrong thing.
Objective acceptance criteria keep the team in sync as they define,
implement,and accept [story cards][].

* A [business analyst][] should believe that a story card has objective acceptance criteria before marking the card as [Approved for Development][story_cards]. 
* A [project sponsor][] should verify the acceptance criteria before approving a card for development.
* A [developer][] should verify the acceptance criteria before accepting a card for development.

We try not to go overboard in documenting the acceptance criteria.
It's possible to keep documenting well beyond the point where the additional
detail ceases to pay for itself.
A good rule of thumb is "the smallest description that a
non-team member could comfortably use to test that a card is complete."

For example, "Basic CRUD functionality for the account object" is too vague. However, "Basic CRUD functionality for account, using the User CRUD story as a guideline" *might* be enough, if the "User CRUD" story has already been accepted.