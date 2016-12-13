---
layout: post
title: Regularization of Inverse Problems- Part II
thumbnail: img/regularization-of-inverse-problems-part-ii.png
buttons:
  - PDF: ../../pdf/ill-posed-linear-operator.pdf
  - LATEX: https://www.overleaf.com/read/yrdrzhhfkdpd
excerpt: In this part we formulate inverse solutions for ill-posed linear operators.
type: project
date: 2016/8/15
anchors:
  - Introduction: introduction
  - Generalized Inverse: moore-penrose-generalized-inverse
  - Compact Linear Operators: compact-linear-operators
  - Spectral Theory : spectral-theory-and-functional-calculus
  - Presentation: presentation
---

### Introduction

In this part we will formulate the concept of ill-posedness for linear operators more formally.
Based on the previously learnt Hadamard's conditions for well-posedness, we formulate an ill-posed
problem in terms of a linear operator.

### Moore-Penrose Generalized Inverse

Now, let the operator $$ T $$ be mapped from Hilbert space $$ X $$ to $$ Y $$.We would like to define
some sort of solution for the inverse of this operator, even at points not originally in the
range of $$ T $$. Hence, we define the Moore-Penrose Generalized Inverse.

We define all x having that quality that
$$
\begin{equation}
\left\| Tx-y \right\| =inf\{ \left\| Tx-y \right\| | x\in X\}
\end{equation}
$$
as least-square solutions. To fight the problem of uniqueness of solution we further define the
best-approximate solution to be the least-square solution of the minimum norm.

As it turns out, the Moore-Penrose Generalized Inverse is actually the best-approximate solution
( Only for points $$ y \in D(T^\dagger )$$, where $$ T^\dagger $$ is the Moore-Penrose Generalized Inverse )

### Compact Linear Operators

We study Compact Linear operators since integral operators are compact under suitable assumptions.
Compact linear operators give us a lot of functionality in reformulating our solutions. For selfadjoint
linear operator we define the $$ \textit{Eigensystem} ({\lambda }_{n};{v}_{n}) $$, and for
compact linear operators that are not self-adjoint, we define the singular system  we construct
a $$ \textit{singular system} ({ \sigma }_{n};{v}_{n},{u}_{n}) $$.

Using these definitions, we derive important results and also show the link to Picard's Criterion, which
states that >A best-approximate solution of $$ Kx = y $$ exists only if the generalized Fourier coefficients
($$ \left<y,{u}_{n}\right> $$) decay fast enough relative to $$ {\sigma}_{n} $$.

### Spectral Theory and Functional Calculus

Now, We define the spectral family $$ E_\lambda $$, the spectral integral of our solution and formulate
important theorems and propositions. These are fun to prove and will be very useful ahead.

### Presentation

For going through the actual latex presentation,

* Download the PDF [here](../../pdf/ill-posed-linear-operator.pdf)

* See the latex code [here](https://www.overleaf.com/read/yrdrzhhfkdpd)
