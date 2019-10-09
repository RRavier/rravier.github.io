---
title: 'Quantifying Gerrymandering: A Case Study of Redistricting in North Carolina'
collection: papers
projectName: gerrymandering
permalink: /projects/gerrymandering/Quantifying
tags:
  - Redistricting
  - Outlier Analysis
  - North Carolina
---


North Carolina has a storied history with gerrymandering. The 2016 congressional redistricting was accused of being a partisan gerrymander, in part due to the discrepancy between the statewide popular vote (close to a 50/50 split between Republicans and Democrats) to the actual outcome (9 Republicans and 4 Democrats) in 2016. Given the geographical nature of the problem, this is not clear: **can we quantify the extent of the gerrymandering in an interpretable way?**

{% include base_path %}
{% assign NCURL = base_path | append: '/projects/gerrymandering/Quantifying' %}
{% assign samsCodeURL = base_path | append: '/code/SAMS' %}

The analysis present in this work came from a 2016 summer project for Duke's [Data+ Program](bigdata.duke.edu/data), which itself was a continuation of other undergraduate research efforts previously performed. The original goal was to develop rigorous evidence to determine whether a given redistricting was a partisan gerrymandering; to do this, an MCMC scheme was used various redistrictings of North Carolina based on a Gibbs measure that took into account traditional redistricting criteria: as equal as possible population, geographic compactness, VRA satisfaction, and preservation of municipal (county) boundaries. This work introduced a number of important ideas in the study of partisan gerrymandering , namely:

* Basing quantitative analysis with respect to a sampled ensemble of redistricting plans rather than global baselines, as done with past measures such as the efficiency gap.

* Interpretable plots that can easily illustrate whether a given redistricting plan is a partisan gerrymander


The initial version of this work can be found [here](arxiv.org/abs/1704.03360), and the updated version in preparation for journal submission can be found [here](arxiv.org/abs/1801.03783). My primary role in this paper was as a summer mentor for Han Sung and Justin.