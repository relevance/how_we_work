---
permalink: developer_narrative.html
layout: toc
title: The Developer View
gh-filename: developer_narrative.md
---
Use numbered headers: true

* This will become a table of contents (this text will disappear).
{:toc}

# The Developer View

This document addresses the way Relevance works from the perspective of a [developer][].
A developer might be someone who writes code, or it may be an interaction designer,
a graphic designer, or a tester.

In essence, this document describes the things that happen *in between* the daily standup meetings.
Put another way, the developer view addresses those activities that don't usually require direct involvement
by customers and other stakeholders.

That means that developers *must* have a clear understanding of the larger context in which these
activities exist: [the stakeholder view][stakeholder_narrative].
At Relevance, developers and customers collaborate closely.
We follow the process described in that document;
this one is mostly about the practices and standards that developers adhere to.

{% include tools_and_practices.md %}

{% include pair_programming.md %}

{% include tdd_and_bdd.md %}

{% include code_review.md %}

{% include continuous_integration.md %}

{% include code_coverage.md %}

{% include distributed_source_control.md %}

{% include pm_buddy.md %}

{% include open_source_fridays.md %}

{% comment %}

## Topics that should be mentioned, with primary coverage elsewhere

* audits
* business analyst
* daily standup
* discretion
* facilitator
* iteration planning
* iterations
* objective acceptance criteria
* points
* project audit
* project management practices
* project sponsor
* project team
* retrospectives
* risk assessments
* staging
* stakeholder
* story cards

## Other topics that should be included

{% endcomment %}

{% comment %} No content in references.md, just link label definitions {% endcomment %}
{% include references.md %}
