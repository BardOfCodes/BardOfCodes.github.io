---
layout: post
title: Regularization of Inverse Problems- Part I
thumbnail: img/regularization-of-inverse-problems-part-i.png
buttons:
  - PDF: ../../pdf/introduction-inverse-problems.pdf
  - LATEX: https://www.overleaf.com/read/fkxxzvqzcvdp
category: regularization
excerpt: The first in a 5 part introduction to Regularization of Inverse Problems.
type: project
date: 2016/8/1
anchors:
  - Introduction: introduction
  - What are Inverse Problems?: what-are-inverse-problems
  - Demonstration: demonstration
  - Some Examples: some-examples
  - Presentation: presentation
---

### Introduction

Only by the start of this millennia was Data Science established as an independent field in itself. So.
Did mathematicians not think of the problems of seeking information from data before?

As it turns out, these were problems that had been long ago discovered in many experiments in physics.
Viktor Ambartsumian, a Soviet- Armenian physicist, during the 1920s, while studying the theory
 of atomic structures, introduced to concept of Inverse problems. In layman terms, he asked,
 given some observed discrete energy levels in an atomic structure, can we form its equation?
In a cruder form, having observed some data, can we find its relation?

Now, that was in 1920s. After about a century, by the work of great minds like E. H. Moore,
Arne Bjerhammar, Andrey Tikhonov and many more, we now have an extensive theory on the treatment
 of such problems.  From more formal definitions, to strong results to actual practical application,
 the theory of inverse problems now is a vast topic in itself. It has applications in tomography, X-ray
 reconstruction, imaging and many other areas.

To me, this seemed like a very useful and interesting field to study. Hence, under the guidance
 of *Dr. Ankik K. Giri* I took a reading project, on the book “Regularization of Inverse Problems”.
 This book was a joint effort of Heinz Werner Engl, Martin Hanke, and Eric A. Neubaurer. Along the way
 I made Latex presentations to explain the content of each chapter as a one hour lecture.

In this part I would be discussing briefly the Introduction to Inverse problems. This document is based on the 1st chapter of the said book.

### What are Inverse Problems?

Direct problems deal with the issue of, given the parameters and the model, what would be
the outcome? Inverse problems are those problems where we ask, gives the outcome, what is
the value of the parameters? (And sometimes what is the model itself!)

The problem with inverse problems is that they are, almost always, ill-posed. That
makes them much harder to solve.

### Demonstration

Knowledge is best presented in the simplest form. So, to learn why ‘inverse’ problems’ are
worth studying, we go through a brief demonstration of differentiation and integration
from data. Through Integration and differentiation, which are quite basic concepts (on the
surface only, though), we can show the strong differences between a direct problem and an
inverse problem.

### Some Examples

Finally, I covered some inverse problems that we face in the real life.

#### Radon Inversion

When x-rays are passed through an object, the decay in their intensity is proportional to the

* Initial intensity $$ I $$

* The density $$ f $$

* And the distance travelled $$ \delta t $$

We hit the body with X-rays along different directions. Now, the problem at hand is to
determine the density $$f$$ of the object based on the measured initial and final intensities
of the X-rays.

#### Image Reconstruction

Here we deal with the problem of deblurring a blurred image. Blurring is seen as a
convolution operation. Hence we use the Fourier transform to solve the problem.  Only
problem being, it becomes ill-posed in the process.

### Presentation

For going through the actual latex presentation,

* Download the PDF [here](../../pdf/introduction-inverse-problems.pdf)

* See the latex code [here](https://www.overleaf.com/read/fkxxzvqzcvdp)
