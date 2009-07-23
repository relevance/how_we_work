## Staging Environments {#staging}

One of our goals is to get software into production---even if the only early users are a few of the customer's stakeholders---as soon as possible in the development cycle.
However, once early versions of the software are in production,
it would be disruptive to push new-and-not-fully-verified features into the production system,
which may be in active use either for production work or for demonstrations or training for potential users.

Therefore, we set up a second deployment environment, the *staging* environment.
Features that are ["ready for showcase"][story_cards] are deployed first to staging,
where the [project sponsor][] and other [stakeholders][stakeholder] can verify that the features work as expected.
Features that aren't quite ready can be pushed back to development;
others are marked as complete.

At least once an iteration, and more often with customer approval, completed features are pushed to the production environment.
