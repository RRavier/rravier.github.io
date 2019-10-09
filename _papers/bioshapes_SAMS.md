---
title: 'SAMS: Shape Alignment, Mapping, and Statistics'
collection: papers
projectName: bioshapes
permalink: /projects/bioshapes/SAMS
tags:
  - Geometric Morphometrics
  - Surface Registration
  - Statistical Shape Analysis
---

Fully automated methods for statistical shape analysis are needed in order to do high-resolution analysis of large amounts of data. Existing methods primarily focus on the case when shapes are topological spheres and have little variation. SAMS is a package that will work on all simply-connected shapes and can robustly handle higher variability of data.

{% include base_path %}
{% assign codePath = base_path | append: '/code/SAMS' %}

SAMS is detailed [here]({{codePath}}) and is available for download at my [Github repository](https://github.com/RRavier/SAMS). This paper is the formal announcement of SAMS. We show its power by analyzing three different cases of interest in the anthropological realm: two concerning molars, and one concerning talus bones. From a statistical perspective, the most interesting results concern the meaningfulness of the *parametric* local significance tests compared to their nonparametric permutation cousins, giving some justification to the assumption of Gaussianity of the data. This has inspired numerous different research directions.

The paper will be available for download soon.