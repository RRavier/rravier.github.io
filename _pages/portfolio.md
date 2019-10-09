---
layout: archive
title: "Things I've Done"
permalink: /portfolio/
author_profile: true
---

My primary research interest concerns applications of mathematics and machine learning to areas where the rigorous foundations are less than desirable, or where assumptions used in proving theorems and developing learning algorithms for commonly analyzed cases do not hold for data obtained in practice. This leads to a lot of experimental work, all with the aim towards better understanding these problems and developing deployable solutions. 

  Below, you'll see links to the projects I've worked on throughout my career. I find all of these things interesting, and **I hope you do, too.**

## Research Areas
{% include base_path %}

{% for post in site.projects reversed %}
  {% include archive-single.html %}
{% endfor %}
