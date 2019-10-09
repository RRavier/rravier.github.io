---
title: 'Shape Analysis in Evolutionary Biology'
collection: projects
permalink: /projects/bioshapes/
tags:
  - Geometry Processing
  - Statistical Shape Analysis
  - Manifold Learning
---

How much can we learn about biology by looking at anatomical surfaces? Potentially a lot, but there are many preprocessing issues to deal with before we can.

## Summary
Experts in many realms of biology have grown interested in the role of the *shape* of objects of interest. There are many questions that one can ask: exactly what can the shape of an object determine about it? If there are a collection of shapes of the same basic type (i.e. crowns from the same type of molar), are there natural ways in which they cluster? How does this relate to genetic information?

Rigid shapes coming from evolutionary history (e.g. bones and teeth) provide an interesting challenge for mathematics. Shapes of the same basic type coming from multiple different species can exhibit a much wider amount of variation (i.e. are much less isometric) than those coming from just humans. In some cases, this increased variation renders standards tools and methods for computing features, registrations, and shape statistics useless. The goal of this project is to fix these issues and develop new tools that can be used in place of these.

## Projects
{% for post in site.papers reversed %}
    {%if post.projectName == 'bioshapes'%}
        {% include archive-single.html %}
    {%endif%}
{%endfor%}