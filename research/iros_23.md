---
layout: post
title:  Skill Generalization with Verbs
date:   2023-06-06 00:00:00 +0830
categories: research_work
tags: research_work
authors: R. Ma, L. Lam, B. A. Spiegel, <b>A. Ganeshan</b>, B. Abbatematteo, R. Patel, D. Paulius, S. Tellex, G. Konidaris.

abstract: It is imperative that robots can understand natural language commands issued by humans. Such commands typically contain verbs that signify what action should be performed on a given object and that are applicable to many objects. We propose a method for generalizing manipulation skills to novel objects using verbs. Our method learns a probabilistic classifier that determines whether a given object trajectory can be described by a specific verb. We show that this classifier accurately generalizes to novel object categories with an average accuracy of 76.69\% across 13 object categories and 14 verbs. We then perform policy search over the object kinematics to find an object trajectory that maximizes classifier prediction for a given verb. Our method allows a robot to generate a trajectory for a novel object based on a verb, which can then be used as input to a motion planner. We show that our model can generate trajectories that are usable for executing five verb commands applied to novel instances of two different object categories on a real robot. 
venue: IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2023
thumbnail: assets/res/iros_23.png
pub_link: http://irl.cs.brown.edu/pubs/skillgen_verbs.pdf
---

## H2 Abstract:

{{ page.abstract }}