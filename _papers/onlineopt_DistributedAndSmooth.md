---
title: 'Curvature Bounds Improve Online Performance for Distributed Optimization'
collection: papers
projectName: onlineopt
permalink: /projects/onlineopt/DistributedOCOSmoothness
tags:
  - Online Optimization
  - Distributed Optimization
  - Convex Optimization
---

For centralized algorithms, where there is only one agent optimizing, it is known that strong convexity of objective functions improves convergence rates of optimization methods, and thus improves performance guarantees in online scenarios in the centralized setting, *even in the adversarial case*. Distributed methods have multiple agents optimizing a function simultaneously. Can we get similar performance guarantees of online methods in the distributed setting, or will requiring communication of agents destroy any hope?

The answer of the paper is, well, **probably most of the time.** This is an empirical statement more than it is a probabilistic one. In online optimization, error bounds are usually given in terms of quantities that provide summaries of the behavior of the dynamical system of objectives. With plain convexity (i.e. no guarantees on curvature), it is known that the performance bound explicitly depends on the total length of time of the online optimization problem. In the centralized setting, we can get rid of this if we assume strong convexity (which gives a lower bound on the curvature of the objective), basically using the fact that gradient descent is a contraction in the strongly convex setting.

In the distributed setting, we can get rid of this explicit time dependence at the cost of adding terms summarizing evolution of gradients, which is not true of the centralized case. Though one might initially think that these terms could be much more of a severe penalty depending on the case, it is quite possible that they are extremely negligible. What is perhaps most interesting is that these gradient terms cannot, in general, go away, or at least that's what an empirical example highly suggests.

An initial version of this work will appear in CDC 2019, with a more elaborate version to soon follow.
