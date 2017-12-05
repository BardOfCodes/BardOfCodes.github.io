---
layout: post
title: Regularization of Inverse Problems- Part III
thumbnail: img/regularization-of-inverse-problems-part-iii.png
buttons:
  - PDF: ../../pdf/regularization-operators.pdf
  - LATEX: https://www.overleaf.com/read/kkxmvtsmmxrb
excerpt: In this part we learn the formal definition of a regularization method and important results about convergence.
type: project
date: 2016/9/1
anchors:
  - Introduction: introduction
  - Order Optimality: order-optimality
  - Regularization by projection: regularization-by-projection
  - Presentation: presentation
---
### Introduction

In ill-posed problems, $$ T^\dagger y^\delta $$, where $$ y^\delta $$ is the measurement with
noise, is unbounded. Infact, it might not even exist! Hence we look for an approximation $$ x^{\delta}_{\alpha} $$,
such that it depends continuously on the noisy data, and tends to $$ x^\dagger $$ as the
noise level decreases to zero.

With this motive, we formulate a regularization method $$ (R_\alpha , \alpha ) $$, such that it satifies the stated conditions
formally. We also define what we mean by its convergence.

Now, $$ \alpha $$, called the parameter choice rule, can depend on $$ y^\delta $$, data with noise,
and $$ \delta $$, the error levels. We define the various kinds of parameter choice rule
based on its independence $$ y^\delta $$ or $$ \delta $$.

### Order Optimality

As far as the convergence of Regularization methods is concerned, we need to also think about the
rate if this convergence. We can define the rate of convergence as the rate at which,

$$ \begin{equation}
\left\| {x}_{\alpha} - {x}^{\dagger} \right\| \rightarrow 0 \quad
as \quad \alpha \rightarrow 0.
\end{equation}
$$

Along the way we define the modulus of continuity, $$ \Omega(\delta, M) $$, and the worst
error possible under the information that $$ x^\dagger \in M $$, $$ \triangle(\delta,M,R) $$.
Using these two definitions we are able to define the optimal regularization method to be the one
for which,  $$ \triangle(\delta,M,R) $$ is the lowest among all possible scenarios.

Now, to more rigourously using a-priopi information we define source sets, $$ X_\mu $$, and their
source representation in $$ X_{\mu,\rho} $$. Finally we fomulate the important defination
of optimal regularization method which links the a-priori information to the worst error possible.

### Regularization By Projection

The last section covers the regularization method of finite dimensional projection. We discuss this
method now in terms of the definitions that we have made in this chapter, and also find out
its rate of convergence with some a-priori conditions.

### Presentation

For going through the actual latex presentation,

* Download the PDF [here](../../pdf/regularization-operators.pdf)

* See the latex code [here](https://www.overleaf.com/read/kkxmvtsmmxrb)
