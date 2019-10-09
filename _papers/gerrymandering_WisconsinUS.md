---
title: 'The Discovery of the Firewall: Evaluating Partisan Gerrymandering in Wisconsin'
collection: papers
projectName: gerrymandering
permalink: /projects/gerrymandering/Firewall
tags:
  - Firewall
  - Redistricting
  - Wisconsin
---

The word "firewall" is indicative of a structure that prevents something from crossing, as is commonly used when it comes to malware in computers. An analysis of redistricting at the state level in Wisconsin reveals a similar structure.

{% include base_path %}
{% assign QuantURL = base_path | append: '/projects/gerrymandering/Quantifying' %}

The discovery of the firewall came through an analysis of the Wisconsin state legislature contemporary with the U.S. Supreme Court case *Gil v. Whitford.* which is most famous for its ties to the efficiency gap measure, which has since been largely rebuked. The methodolgy used in this analysis is the same MCMC and statistical analysis in the original [Quantifying Gerrymandering in North Carolina]({{QuantURL}}) work.

The firewall behavior is summarized as follows: if we uniformly shift the votes of a given election in a direction that favors a particular party, at some point an increase in favor has minimal to no practical effect on outcome. In the case of Wisconsin, as votes were uniformly shifted to more favor Democrats, the number of seats won practically plateaued at some point. **The Republicans were protected despite an increased percentage of Democrats.**


The results of our analysis, and the evidence of the existence of the firewall can be found on [arXiv](arxiv.org/abs/1709.01596)