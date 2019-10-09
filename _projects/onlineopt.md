---
title: 'Data Driven Online Optimization'
collection: projects
permalink: /projects/onlineopt/

---

Research in optimization has exploded due to increases in computational ability. Online optimization, where objective functions can change in time, is a field with vast potential for both interesting theoretical investigations as well as practical applications well outside areas traditionally considered in, e.g. control and learning communities.

## Summary

My research in this area has been primarily motivated by statistics of time-varying distributions on (potentially) time-varying nonconvex metric spaces (e.g. image and shape manifolds) for which the distributions are not directly observable, but a number of samples at each time are. In this setting, arguably the most canonical of all statistics, the mean, is not defined as usual due to the lack of convexity; it is instead defined as the minimizing point of a functional known as the Fréchet variance. Given that means can be interpreted as "prototypical" examples of data, it then becomes important to better understand the dynamics of optimization problems.

Since the distributions at each time are not directly observable, we need to combine observed data with probabilistic models in order to make approximations of the distributions, hence approximations of the means via conditional expectations given a model class. Models that capture accurately capture these means can give powerful inferential insight to the behavior of various phenomena. Again, as means are defined by optimization problems, this turns into a question of modeling dynamical systems of optimization problems.

Dynamical systems of optimization problems have been studied, though usually under the setting where the problem is smoothly varying in time or under adversarial (i.e. non-predictable) dynamics, neither of which perfectly fits our case. The role of prediction has been studied, but in a much more limited fashion. The standard methodology of this field is to adapt traditional optimization algorithms to online scenarios in obvious manners, and then investigate properties of various performance measures (though, in some cases, you can exploit structure and do things a little different, as is done in predictor-corrector methods).

If you view the work as somewhat incremental, *it's okay. I do, too.* It is important to note that **everything below is more about the interaction of a particular coupling of dynamical systems (objective functions and optimizers) and less about optimization proper.** There is an abundance of potential for future work, but involves much better of understanding of dynamical systems in the proper language of optimization, which is itself a non-trivial task given the difference in appropriate topology.

{% for post in site.papers reversed %}
    {%if post.projectName == 'onlineopt'%}
        {% include archive-single.html %}
    {%endif%}
{%endfor%}