---
layout: post
title:  FDA: Feature Disruptive Attack
date:   2019-10-02 00:00:00 +0830
authors: <b>A. Ganeshan</b>, B. S. Vivek, R. V. Babu
categories: research_work
tags: research_work
abstract: Though Deep Neural Networks (DNN) show excellent performance across various computer vision tasks, several works show their vulnerability to adversarial samples, i.e., image samples with imperceptible noise engineered to manipulate the network's prediction. Adversarial sample generation methods range from simple to complex optimization techniques. Majority of these methods generate adversaries through optimization objectives that are tied to the pre-softmax or softmax output of the network. In this work we, (i) show the drawbacks of such attacks, (ii) propose two new evaluation metrics: Old Label New Rank (OLNR) and New Label Old Rank (NLOR) in order to quantify the extent of damage made by an attack, and (iii) propose a new adversarial attack FDA: Feature Disruptive Attack, to address the drawbacks of existing attacks. FDA works by generating image perturbation that disrupt features at each layer of the network and causes deep-features to be highly corrupt. This allows FDA adversaries to severely reduce the performance of deep networks. We experimentally validate that FDA generates stronger adversaries than other state-of-the-art methods for image classification, even in the presence of various defense measures. More importantly, we show that FDA disrupts feature-representation based tasks even without access to the task-specific network or methodology.
venue: IEEE / CVF International Conference on Computer Vision (ICCV), 2019
thumbnail: assets/res/fda.png
pub_link: https://arxiv.org/abs/1909.04385
website_link: https://bardofcodes.github.io/fda/
code_link: https://github.com/BardOfCodes/fda
---

Our Paper: <a href= 'https://arxiv.org/abs/1909.04385'>"FDA: Feature Disruptive Attack"</a> got accepted in <a href= "http://iccv2019.thecvf.com/">IEEE / CVF International Conference on Computer Vision (ICCV), 2019</a>!


## H2 Abstract:

{{ page.abstract }}