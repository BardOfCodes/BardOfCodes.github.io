---
layout: post
title:  Generalizable Data-free Objective for Crafting Universal Adversarial Perturbations
date:   2018-07-02 00:00:00 +0830
authors: K. M. Reddy*, <b>A. Ganeshan*</b>, R. V. Babu
categories: research_work
tags: research_work
abstract: Machine learning models are susceptible to adversarial perturbations. small changes to input that can cause large changes in output. It is also demonstrated that there exist input-agnostic perturbations, called universal adversarial perturbations, which can change the inference of target model on most of the data samples. However, existing methods to craft universal perturbations are (i) task specific, (ii) require samples from the training data distribution, and (iii) perform complex optimizations. Additionally, because of the data dependence, fooling ability of the crafted perturbations is proportional to the available training data. In this paper, we present a novel, generalizable and data-free approaches for crafting universal adversarial perturbations. Independent of the underlying task, our objective achieves fooling via corrupting the extracted features at multiple layers. Therefore, the proposed objective is generalizable to craft image-agnostic perturbations across multiple vision tasks such as object recognition, semantic segmentation, and depth estimation. In the practical setting of black-box attack scenario (when the attacker does not have access to the target model and it's training data), we show that our objective outperforms the data dependent objectives to fool the learned models. Further, via exploiting simple priors related to the data distribution, our objective remarkably boosts the fooling ability of the crafted perturbations. Significant fooling rates achieved by our objective emphasize that the current deep learning models are now at an increased risk, since our objective generalizes across multiple tasks without the requirement of training data for crafting the perturbations. To encourage reproducible research, we have released the codes for our proposed algorithm.
venue: IEEE Transactions on Patter Analysis and Machine Intelligence, 2018
thumbnail: assets/res/gduap.png
pub_link: https://arxiv.org/abs/1801.08092
website_link: https://val-iisc.github.io/GD-UAP/
code_link: https://github.com/val-iisc/GD-UAP
---

Our Paper: <a href= 'https://arxiv.org/abs/1801.08092'>"Generalizable Data-free Objective of crafting Universal Adversarial Perturbations"</a> got accepted in <a href= "https://ieeexplore.ieee.org/xpl/mostRecentIssue.jsp?punumber=34&filter=issueId%20EQ%20%224359286%22&pageNumber=2">IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI)</a>!


## H2 Abstract:

{{ page.abstract }}