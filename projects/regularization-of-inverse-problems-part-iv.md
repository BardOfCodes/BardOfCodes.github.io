---
layout: post
title: Regularization of Inverse Problems- Part IV
thumbnail: img/regularization-of-inverse-problems-part-iv.png
buttons:
  - PDF: ../../pdf/continuous-regularization-methods-1.pdf
  - LATEX: https://www.overleaf.com/read/qhcphdnnxskn
excerpt: Now its time to look into some of the choices of the parameter choice rule, a-priori parameter choice and the Discrepancy principle.
type: project
date: 2016/9/15
anchors:
  - Introduction: introduction
  - Saturation and Converse result: saturation-and-converse-result
  - The Discrepancy Principle: the-discrepancy-principle
  - Presentation: presentation
---

### Introduction

First, we will consider the class of linear regularization methods based on spectral theory
for self-adjoint operators. We see that $$ x^\dagger $$ depends on $$ 1/ \lambda $$ which has
pole in $$ 0 $$. We introduce the parameter-dependent family of functions $$ g_\alpha (\lambda) $$,
which are atleast piecewise continuous in the required domain. We also define the parameter-dependent
family of functions $$ r_\alpha (\lambda) $$, which are linked to the residual $$ x^\dagger - x_\alpha $$

Based on these definitions, we find out what a-priori information is required for convergence of
these methods. Once their convergence is guarenteed, we formulate the conditions required for
optimal convergence.

### Saturation and Converse result

An interesting phenomenon is that some regularization methods give optimal rate of convergence
 only for values of $$ \mu $$ upto a specific $$ \mu_0 $$, where $$ \mu $$ is the same are the
 $$ \mu $$ in  $$ X_{\mu,\rho} $$. The term saturation is used to describe this behaviour.

When we try to imply the existence of a $$ x^\dagger $$ in $$ X_\mu $$, through the convergence
rate, it is known as converse result. Converse results are of practical importance as it helps
us to understand where the solution $$ x^\dagger $$ will lie.

### The Discrepancy Principle

This principle was discovered my Marozov, and is a a-posteriori parameter choice rule.The
regularization parameter defined via the $$ \textit{Discrepancy Principle} $$ is

$$
\begin{equation}
\alpha (\delta,{y}^{\delta}) = sup \{ \alpha > 0 \mid \left\| T{x}^{\delta}_{\alpha} -{y}^{\delta} \right\| \le \tau \delta \}
\end{equation}
$$

The intuition behind it is that since the data error itself is of the magnitude of $$ \delta $$,
asking of the approximate solution $$ \hat{x} $$ with discrepancy less that $$ \delta $$ is not sensical.
hence, a residual of the order of $$ \delta $$ is the best we can ask for.

### Presentation

For going through the actual latex presentation,

* Download the PDF [here](../../pdf/continuous-regularization-methods-1.pdf)

* See the latex code [here](https://www.overleaf.com/read/qhcphdnnxskn)
