---
title: 'Prediction in Online Convex Optimization: The Parametrizable Setting'
collection: papers
projectName: onlineopt
permalink: /projects/onlineopt/ParameterPredictionOCO
tags:
  - Online Optimization
  - Predictive Methods
  - Model selection
---

Online convex optimization (OCO) problems typically focus on adversarial scenarios. Many, however, aren't. If you know this, and have some reasonable model of your future, what improvements can you get? Furthermore, how well can you do if you're starting from scratch?

From a practical perspective, an oft-overlooked assumption for time-varying optimization problems is the *source* of the time-varying component. In many cases (tracking, finance, etc.) this stems from some dynamical parameter; Generally, the particular objective function has fixed algebraic form, but various parameters change. This assumption still allows for extremely general cases via representing objectives as functional time series can be obtained. 

The inspiration of [this CDC 2019 paper](arxiv.org/abs/1901.11500) was to propose an interesting line of study combining functional time series, which itself is also reduced down to the problem of (practically finite-dimensional) vector time series. The theoretical assumptions in this work are somewhat strong (in particular, the Lipschitz continuity of the gradients on the parameter) but purposeful so as to better illustrate that successful parameter prediction leads to improvement of regret metrics. That being said, it's not clear if you could relax this assumption much while still giving a meaningful performance measure (realistically some amount of local Hölder continuity), and it holds in very general cases. Better understanding of these estimates can be made by adding slightly more structure, though for purposes of page limits and traditional form of analysis in OCO, we did not do this, though it is clear that these would be of immediate future interest. In particular, it is useful to note that these bounds are in terms of parameter estimation error, which is much easier to study and understand than, say, gradient estimation error.

For practical purposes, we also developed and performed basic analysis on a meta-learning model that proposes combining model selection for the governing data-processes with optimization algorithms. It is unclear if, in general, these estimates could be improved, but it is most certainly possible/of interest to do so for explicit cases of models. The synthetic examples are simple and illustrate the idea of the algorithm. The example on financial data is a favorite of mine that attempts to illustrate that even displaying some effort can be better than none.

**It is important to note that the ideas proposed in this paper apply in general to more situations than evaluated in this paper.** You can use your favorite optimization algorithm, the performance will carry over appropriately. Again, this paper was more about the *idea* and less about the technical details.
