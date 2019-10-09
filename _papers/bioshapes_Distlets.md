---
title: 'Distlets: Building Flexible, Interpretable Dictionaries for Shape Data'
collection: papers
projectName: bioshapes
permalink: /projects/bioshapes/Distlets
tags:
  - Dictionary Learning
  - X-lets
  - Metric Embeddings
---
The geometric and topological properties of spaces of shapes are not well understood, let alone those of anatomical surfaces. However, those of other spaces (e.g. Hilbert spaces) are. If we were able to embed shapes into a nicer, lower dimensional space, we could use pullbacks of tools on the nicer spaces to learn more about shape spaces. Sparse dictionaries provide a natural, interpretable way to do this.

Dictionary learning has been a vital tool in digital signal processing, in particular image analysis. To build an effective dictionary, atoms must be able to capture both isotropic and anisotropic features. Wavelets, ridgelets, and curvelets are powerful atoms for constructing dictionaries on images with desirable theoretical properties whose proofs depend largely on those of the Euclidean Fourier transform; these constructions immediately break down on general shapes in non-recoverable ways.

Wavelets did not suffer the same fate given their lack of directionality; wavelets can be defined on triangular meshes (embedded 2-simplices with triangular faces) via a generalization of convolution to graphs as well as via a lifting scheme provided that the connectivity structure is sufficiently regular. The directionality. Graph convolutions do not have analogous properties to those used to construct ridgelets and curvelets, and in general we cannot assume that meshes seen in practice have enough regularity in their triangulations to consider any potential adaptation of the lifting scheme.

Despite these failures, it is still of practical interest to construct dictionaries that capture anisotropic features on surfaces. We can do this in a manner analogous to by recalling the definition of the ridgelet: given a hyperplane, a ridgelet is a function that is constant on all parallel hyperplanes whose graph along any line transverse to these hyperplanes is a waveform satisfying particular decay and moment properties. Using coordinate charts, one could directly define these adaptations of these by including additional decay terms. From a practical standpoint, this could be very cumbersome and, depending on the waveform used, be completely impractical. If, however, we restrict to **symmetric** waveforms (and are willing to potentially sacrifice some smoothness and moment properties which don't matter in practice), we can build dictionary elements by ignoring coordinate charts and having the value of the function be based solely on the distance to a given feature, which is easy to compute quickly. Hence, we term these elements *distlets.*

Limiting the amount of computations still presents itself as an issue, but we cannot use the same types of tricks as in fast transforms for 1-D signals and images; such methods require regularity of the discretization structure, which we do not assume. As an alternative, we can instead use clever sampling techniques to dramatically reduce the search space of features about which to construct dictionary elements. These dictionaries can produce meaningful results; using such dictionaries to learn representations of meshes with thousands of points via basis pursuit, **the Euclidean distance on the vectors of coefficients is the same as the Procrustes distance on the shapes!**

The paper will be available for download soon.