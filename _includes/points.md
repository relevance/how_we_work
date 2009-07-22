### Story Points {#points}

Our story and task estimates are not expressed in hours or days; they're expressed in *points*.
This acknowledges the inevitability of error in estimates, and of varying productivity,
helping to avoid mismatches in expectations between Relevance and our customers.

At the level of tasks, estimates are kept separate from explicit notions of time.
But at the level of iterations, points are mapped back onto time using the concept of
[velocity][]: the number of estimated points that
we achieve in a single iteration.
(That's one reason we like to stick to two-week iterations except when it's
absolutely necessary to vary the iteration length.
If all iterations are two weeks long, it makes velocity numbers directly comparable and much more useful.)

Points and velocity are vital concepts.
As Relevance founder Stu Halloway points out, variance in productivity (or accuracy of estimation)
is like the weather, whereas velocity is like climate.
That it's raining and windy today might be an annoyance, but it's no reason to pack up and move
to another state unless it's like this *every* day.
Similarly, every programmer (and every team) will have days that aren't as productive as we'd like,
but we'll also have days where we really rock.

What matters much more is the climate: how fast we're moving iteration-by-iteration,
moving toward getting the project complete.

### Point values {#point_values}

One aspect of our point estimates sometimes strikes our customers as odd.
(Some have even thought we were joking!)
Only some values are allowed as estimates;
specifically, numbers in the Fibonacci sequence (1, 2, 3, 5, 8, ...).
Why would we do such a silly thing?

As tasks get larger, we have much less confidence in our estimates.
It's more difficult to grasp the full requirements,
and to think about all of the implementation pieces that will be required.
That means that it's also easier for unknown complexities or problems to lurk in such tasks.
So as the size of the task grows, we force the estimates to fit a coarser granularity,
acknowledging the greater likelihood of error.

What are the benefits?

First, it saves time we might otherwise spend arguing about whether a task is (say) 5 points or 6.
Once we get to that size, it could just as likely be either.

Second, it helps us to resist natural pressure to estimate aggressively.
"Surely it's not really an 8," someone might say---and
if we could just knock it down to a 7 we might be tempted,
but a 5 is clearly ridiculous, so it stays an 8.
We'd rather come in under our estimates than exceed them.
(That's not just vanity, or striving to impress---it's also much less disruptive to our customers' plans.)

Finally, it gives us an incentive to subdivide tasks,
making them small enough for more accurate estimates.
We've seen many times how smaller tasks are easier to estimate, develop, test, and track.
(In fact, we won't permit a task larger than 8 points to stand;
those get split right away.
And even 8-point tasks must be split before development on them begins.)

### Velocity {#velocity}

The number of points that are targeted for work in the new iteration is based on the *velocity*
from prior iterations:
the number of estimated points that were actually achieved during those iterations.
The notion of velocity helps us to calibrate the combination of our productivity and
our estimation skill, both of which are variable in specific instances, but mostly stable
in aggregate.
That means that, after the first iteration or two, we can make fairly accurate predictions
of how much work can be done over a certain period of time, allowing the customer to budget
and plan more easily.
