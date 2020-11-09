---
layout: post
title:  Object Pose Estimation from Monocular Image using Multi-View Keypoint Correspondence
date:   2018-08-10 00:00:00 +0830
categories: research_work
tags: research_work
authors: J. N. Kundu*, <b>A. Ganeshan*</b>, M. V. Rahul*, R. V. Babu
abstract: Understanding the geometry and pose of objects in 2D images is a fundamental necessity for a wide range of real world applications. Driven by deep neural networks, recent methods have brought significant improvements to object pose estimation. However, they suffer due to scarcity of keypoint/pose-annotated real images and hence can not exploit the object's 3D structural information effectively. In this work, we propose a data-efficient method which utilizes the geometric regularity of intraclass objects for pose estimation. First, we learn pose-invariant local descriptors of object parts from simple 2D RGB images. These descriptors, along with keypoints obtained from renders of a fixed 3D template model are then used to generate keypoint correspondence maps for a given monocular real image. Finally, a pose estimation network predicts 3D pose of the object using these correspondence maps. This pipeline is further extended to a multi-view approach, which assimilates keypoint information from correspondence sets generated from multiple views of the 3D template model. Fusion of multi-view information significantly improves geometric comprehension of the system which in turn enhances the pose estimation performance. Furthermore, use of correspondence framework responsible for the learning of pose invariant keypoint descriptor also allows us to effectively alleviate the data-scarcity problem. This enables our method to achieve state-of-the-art performance on multiple real-image viewpoint estimation datasets, such as Pascal3D+ and ObjectNet3D. To encourage reproducible research, we have released the codes for our proposed approach.
venue: Geometry Meets Deep Learning Workshop, at ECCV 2018.
thumbnail: assets/res/eccvw.png
pub_link: https://arxiv.org/abs/1809.00553
code_link: https://github.com/val-iisc/pose_estimation
---

Our Paper: <a href= 'https://arxiv.org/abs/1809.00553'>"Object Pose Estimation Using Multi-View Keypoint Correspondence"</a> got accepted as a poster paper in <a href= "https://sites.google.com/site/deepgeometry2018/">The 3rd Geometry Meets Deep Learning Workshop, </a> ECCV'2018!

## H2 Abstract:

{{ page.abstract }}