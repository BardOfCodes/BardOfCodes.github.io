---
layout: post
title:  Improving Unsupervised Visual Program Inference with Code Rewriting Families
date:   2023-06-10 00:00:00 +0830
categories: research_work
tags: research_work
authors: <b>A. Ganeshan</b>, R. Kenny Jones and Daniel Ritchie

abstract: Programs offer compactness and structure that makes them an attractive representation for visual data. We explore how <i>code rewriting</i> can be used to improve systems for inferring programs from visual data. We first propose Sparse Intermittent Rewrite Injection(<b>SIRI</b>), a framework for unsupervised bootstrapped learning. SIRI sparsely applies code rewrite operations over a dataset of training programs, injecting the improved programs back into the training set. We design a family of rewriters for visual programming domains - Parameter Optimization (PO), Code Pruning (CP), and Code Grafting (CG). For three shape programming languages in 2D and 3D, we show that using SIRI with our family of rewriters improves performance - better reconstructions and faster convergence rates, compared with bootstrapped learning methods that do not use rewriters or use them naively. Finally, we demonstrate that our family of rewriters can be effectively used at test time to improve the output of SIRI predictions. For 2D and 3D CSG, we outperform or match the reconstruction performance of recent domain-specific neural architectures, while producing more parsimonious programs that use significantly fewer primitives.
venue: <b> Oral (1.8%)</b> IEEE / CVF International Conference on Computer Vision (ICCV), 2023
thumbnail: assets/res/iccv_23.png
pub_link: https://arxiv.org/abs/2309.14972
website_link: https://bardofcodes.github.io/coref/
---

## H2 Abstract:

{{ page.abstract }}