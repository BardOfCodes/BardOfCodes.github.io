---
layout: post
title: Regularization of Inverse Problems- Part V
thumbnail: img/regularization-of-inverse-problems-part-v.png
buttons:
  - PDF: ../../pdf/continuous-regularization-methods-2.pdf
excerpt: In this part, we exlore an improved parameter choice rule, and heuristic rules.
type: project
date: 2016/10/1
anchors:
  - Improved-A-posteriori Rules: improved-a-posteriori-rules
  - Heuristic Parameter Choice Rules: heuristic-parameter-choice-rules
  - Presentation: presentation
---

### Improved-A-posteriori Rules

In the previous part, the a-posteriori parameter choice rule that we defined, The discrepancy
principle, was optimal only upto $$ \mu_0 -1/2 $$, where $$ \mu_0 $$ is the qualification
of the regularization method.

Now, we define an imporved a-posteriori rule which yeilds optimality upto the qualification
$$ \mu_0 $$ itself. After simpfication it leads to

$$
\begin{equation}
\frac{\partial}{\partial \alpha}({ || r^\alpha ({T}^{*}T){x}^{\dagger} || }^{2} + C
{\delta}^{2} {G}_{\alpha}) =0.
\end{equation}
$$

We prove its optimality, and also show its relation to the discrepancy rule.

###  Heuristic Parameter Choice Rules

In real life, many times the noise level information is not availible. In such situations, we
are forced to use Error-free parameter choice rules, which do not depend on the data error
level $$ \delta $$.Most heuristic rules for error free parameter choice rules are based on
some kind of error estimation. Here we discuss generalized cross-validation and L-curve method.

In one method we pick regularization parameter as the one for which

$$
\begin{equation}
\frac{1}{\alpha}r_\alpha ({T}^{*}T)(y^\delta - y) \quad vs. \quad
g_\alpha ({T}^{*}T){T}^{*}(y_\delta - y)
\end{equation}
$$

In another method, we plot $||{\xalde}||$ versus $||{y^\delta - T {x}_{\alpha}^{\delta}}||$ in a log-log scale
for a large range of $\alpha$ values, and find the 'corner' of the drawn curve. We also cover
Hansen and O'leary Algorithm.

### Presentation

For going through the actual latex presentation,

* Download the PDF [here](../../pdf/continuous-regularization-methods-2.pdf)

* See the latex code [here](https://www.overleaf.com/read/xgwdynqkcqff)
