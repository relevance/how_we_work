---
permalink: stakeholder_narrative.html
layout: toc
title: The Stakeholder View
gh-filename: stakeholder_narrative.md
---
Use numbered headers: true

* This will become a table of contents (this text will disappear).
{:toc}

# The Stakeholder View

This page describes the various pieces of how Relevance builds software,
from the point of view of a stakeholder, rather than of a developer.

(There are a lot of links in this document: some of them to other places
within this page, some to other pages on the site, and some to external
resources.
But the document is designed to be read straight through.
Please don't be distracted or diverted by the links on your first reading;
they're there for easy reference later on.)

We'll begin by defining, in very simple terms, the overall philosophy that
(we believe) makes Relevance's approach to software development work.
Then we'll define roles more precisely, and continue with project
structure and practices, from the overall view down to the day-to-day.

{% include philosophy.md %}

## Roles

Dividing people into two roles---stakeholder and developer---is somewhat arbitrary,
so we'll start by being clear: what is a stakeholder?
And what are some of the more specific roles that a stakeholder might fill?

{% include stakeholder.md %}

{% include project_sponsor.md %}

{% include business_analyst.md %}

{% include project_manager.md %}

{% include developer.md %}

{% include qa.md %}

{% include facilitator.md %}

{% include project_team.md %}

{% include project_management_practices.md %}

{% include discretion.md %}

## Iterations and Stories

The most important concepts in our process are *iterations* (the unit of planning and delivery)
and *stories* (the unit of estimation, development, and tracking).

{% include iterations.md %}

{% include story_cards.md %}

{% include objective_acceptance_criteria.md %}

{% include points.md %}

## Meetings

We try not to spend time in meetings unless the meeting is really
necessary, but of course some kinds of communication are best done
in meetings.  These are the kinds of meetings that occur regularly
on a Relevance project:

{% include daily_standup.md %}

{% include iteration_planning.md %}

{% include risk_assessments.md %}

{% include retrospectives.md %}

{% include audits.md %}

{% include project_audit.md %}

{% include performance_audit.md %}

{% include security_audit.md %}

{% include technical_debt.md %}

{% include staging.md %}

{% comment %}

## Topics that should be mentioned, with primary coverage elsewhere

* code coverage
* code review
* continuous integration
* development practices
* open-source fridays
* pair programming
* performance audit
* pm buddy
* security audit
* tdd and bdd
* tools and practices

## Other topics that should be included

{% endcomment %}

{% comment %} No content in references.md, just link label definitions {% endcomment %}
{% include references.md %}
