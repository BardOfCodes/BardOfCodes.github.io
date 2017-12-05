---
layout: post
title: Waitlist Analysis - "The Big Reveal" Competition entry
thumbnail: img/waitlist_analysis.jpg
buttons:
  - POSTER: ../waitlist_analysis.jpg
  - PREZI: ../rar/waitlist_analysis.rar
category: Data Science
excerpt: This was our prize winning(3rd) submission in "The Big Reveal", a competition organised by Fuzzy Logix, in Congizance'16.
type: project
date: 2016/3/1
anchors:
  - Introduction: introduction
  - The Indian Railways: the-indian-railways
  - The Proposed Improvements: the-proposed-improvements
  - The Proposed Model: the-proposed-model
  - Additional Links: additional-links
---
<img src ="../../img/waitlist_analysis.png" style="margin-left:auto;margin-right:auto;" />

### Introduction

Cognizance, the annual technical festival of IIT Roorkee, is an agglomeration of over 200
events which encompass every wavelength of an entire technical spectrum. Commenced in 2003,
ognizance has emerged as the one of the largest festival of its kind in the Indian subcontinent
and many of its core events witness a participation numbering in thousands.

In 2016, in collaboration with Fuzzy Logix, this competition was organised. With cash prize worth
 Rs. 1 Lac, it was one of the central event. I entered this competition with my two friends,
 Mayank Gupta and Yash Vardhan Chaturvedi.

The goal was to draw a plan that would use the big-data analysis to solve important problems
in one of the selected fields. The options were, healthcare, warfare, Indian railway system, and
a few more. Having travelled in trains way too many times, we thought The Indian Raiways could truly
be revamped with the help of Data Analysis.

We made the presentation in Prezi, to make it more interactive.

### The Indian Railways

The Indian Railways is the second largest network in the world. It is the backbone of our economy.
However, Almost 70% of the trains are delayed, and many passenger trains even run a massive loss. This
problem was a plague for the industry and for a strong economy, it meeded a quick resolution.

Since, we are not the only people aware about these problems, The government of India plans to institute
the Special Unit for Transportation Research and Analysis (S.U.T.R.A.). The plans were revealed in 2016-17
union budget. The Government revealed that the Indian Railways collect over 100TB of data every day.
Hence this seemed like the perfect problem to solve using Big-Data Analysis.

We saw that using data science we could personalize the Indian Railways, providing a better customer
experience, increase reliability and improve resource utilization.Due to time constraints we decided
to focus on one area of the problem, that is the waitlist analysis.

### The Proposed Improvements

Using Waitlist data, we can bring a lot of useful insights.

* We can show the customer the chances or probability of clearance. Coupled with this we can also break the journey into
smaller parts and suggest alternate routes.

* On an increase of demand the Indian Railways, attach extra coaches to existing train. This can be more
accurately modelled. Using Waitlist analysis we can directly infer the need for such an action.

* Due to the diverse nature of the demand of railway system accross the country, it is a hard task to determine
which region would require addition tracks as well as trains. This is again a problem that can be solved from data analysis.

### The Proposed Model

We also had to include a summary of the models which will achieve these proposed imporvements.
We proposed using Random Forest to predict the Waitlist Limit, a regression model for predicting the
Maximum expected Waitlist. We could use independent variables like total train seats, class of travel,
weather data etc.

### Additional links

Now, in hindsight, it was a pretty simple and naive model. However, it was a lot of fun to deliver it
in the time constraints that we had.You can

* Download the Prezi [here](../../rar/waitlist_analysis.rar).

* Download the Poster [here](../../waitlist_analysis.jpg).
