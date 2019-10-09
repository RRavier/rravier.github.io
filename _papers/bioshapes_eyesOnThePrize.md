---
title: 'Eyes on the Prize: Improving Registration via Forward Propagation'
collection: papers
projectName: bioshapes
permalink: /projects/bioshapes/eyesOnThePrize
tags:
  - Geometry Processing
  - Surface Registration
  - Manifold Learning
---

Fully automated registration of shapes can prove to be extremely challenging if the shapes have clearly corresponding parts but wildly different features. 

The probable reason for this stems from such pairs of shapes having different features, causing algorithms to mismatch different areas on the shapes. Empirical observations suggest that better quality correspondences between very different shapes can be obtained by using compositions of correspondences between shapes that are more similar to one another in place. There is not, however, a clear condition on how to choose "good" compositions in practice, let alone one.

This work addresses this question by considering a natural model for the correspondence problem based in differential geometry. More precisely, we can model correspondences between two shapes as parallel transports between two points on a manifold, where correspendences coming from competitions are parallel transports along different paths on the manifold. If we further assume that 

* The true correspondence is the one corresponding to the parallel transport operator from the geodesic (intuitively, this says that shapes evolve "efficiently"), 

* We have rudimentary distance information between all shapes

* There is some procedure that allows us to build the true correspondence map given a finite number of correct initial corresponding points

Then we can introduce simple conditions such that paths (compositions) satisfying these conditions, under reasonable assumptions on the model, give parallel transports close to that of the geodesic. We then these conditions/paths to construct robust algorithm to improve pairwise correspondences between all shapes in a collection, and it is not hard to modify this algorithm to give a robust algorithm for giving *consistent* correspondences for an entire collection of shapes (i.e. specifying one point on one shape unambiguously defines a corresponding point on all shapes).

The paper can be found on [arXiv](www.arxiv.org/abs/1812.10592). 

{% include base_path %}
{% assign samsPaperURL = base_path | append: '/projects/bioshapes/SAMS' %}
{% assign samsCodeURL = base_path | append: '/code/SAMS' %}

The methods developed in this paper can be found in the SAMS method outlined on this website, which can be found on the [paper page]({{samsPaperURL}}), the [project page]({{ samsCodeURL}}), and the [Github repository](www.github.com/RRavier/SAMS).