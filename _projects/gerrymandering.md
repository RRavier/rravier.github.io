---
title: 'Quantitative Foundations of Partisan Gerrymandering'
collection: projects
permalink: /projects/gerrymandering/
tags:
  - MCMC
  - Hypothesis Testing
  - Data Science
---

Partisan gerrymandering is a phenomenon in American politics that, unlike racial gerrymandering, is poorly understood.

## Summary

The United States performs a census every ten years to determine both its total population and the population of each state. Each state is assigned a number of representatives for the US House based on its relative population. Each of these representatives is assigned a geographic area of the state known as a district. There are two main requirements in drawing these districts: each district in a state must have as equal as possible population, and no district can violate the [Voting Rights Act](en.wikipedia.org/wiki/Voting_Rights_Act_of_1965) (VRA). Otherwise, there are no rules at the federal level; **each state can choose how draw districts as they please.** This has allowed for districts to be drawn in a way that influences the outcome: this is known as gerrymandering. This does not just apply to congressional redistrictings, but ones for state legislatures as well.

As a result of the VRA, *racial* gerrymandering, where districts are drawn so as to affect the influence of racial minorities in a state, has been well-established to be illegal. The legality of *partisan* gerrymandering, where districts are drawn so as to affect the influence of a political party, is much more ambiguous. Though the U.S. Supreme Court recently ruled in *Rucho v. Common Cause* that no objective standard for testing partisan gerrymandering exists, meaning that federal courts cannot resolve issues, this does not prevent *state* courts from ruling on partisan gerrymandering cases. There has thus been significant interest to better understand partisan gerrymandering from a quantitative perspective, and develop rigorous metrics and methodologies for determining whether a given redistricting is a partisan gerrymander.

The main methodologies used in this field are based on using Markov chains to perform some sort of significance testing based on ensembles of redistrictings of a state. My work in this area concerns using MCMC methods to perform a global sampling of redistrictings using traditionally valued redistricting criterion, and then subsequently computing a number of statistics on these samplings to get an idea as to whether a given district plan of a state is a statistical outlier with respect to these sampled distributions. This has led to the development of a number of visualizations and the discovery of a number of signals illustrating mechanisms of partisan gerrymandering as well as evidence showing the importance/lack thereof of incorporating traditional redistricting criterion in any analysis.

My participation in this effort has mostly been in a support role; Greg Herschlag, Jonathan Mattingly, a large number of undergraduates, and others have done and are continuing to do an extraordinary amount of quality work in this area. Below you will find many of the results of my participation in these efforts. The [Duke Quantifying Gerrymandering Webpage](sites.duke.edu/quantifyinggerrymandering/) is the digital home of this team.

## Projects
{% for post in site.papers reversed %}
    {%if post.projectName == 'gerrymandering'%}
        {% include archive-single.html %}
    {%endif%}
{%endfor%}
