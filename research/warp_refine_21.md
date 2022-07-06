---
layout: post
title:  Warp-Refine Propagation Semi-Supervised Auto-labeling via Cycle-consistency
date:   2021-10-06 00:00:00 +0830
categories: research_work
tags: research_work
authors: <b> A. Ganeshan </b> , Alexis Vallet, Yasunori Kudo, Shin-ichi Maeda, Tommi Kerola, Rares Ambrus, Dennis Park, Adrien Gaidon
abstract: Deep learning models for semantic segmentation rely on expensive, large-scale, manually annotated datasets. Labelling is a tedious process that can take hours per image. Automatically annotating video sequences by propagating sparsely labeled frames through time is a more scalable alternative. In this work, we propose a novel label propagation method, termed Warp-Refine Propagation, that combines semantic cues with geometric cues to efficiently auto-label videos. Our method learns to refine geometrically-warped labels and infuse them with learned semantic priors in a semi-supervised setting by leveraging cycle consistency across time. We quantitatively show that our method improves label-propagation by a noteworthy margin of 13.1 mIoU on the ApolloScape dataset. Furthermore, by training with the auto-labelled frames, we achieve competitive results on three semantic-segmentation benchmarks, improving the state-of-the-art by a large margin of 1.8 and 3.61 mIoU on NYU-V2 and KITTI, while matching the current best results on Cityscapes.
venue: IEEE / CVF International Conference on Computer Vision (ICCV), 2021
thumbnail: assets/res/warp_refine_21.png
pub_link: https://openaccess.thecvf.com/content/ICCV2021/html/Ganeshan_Warp-Refine_Propagation_Semi-Supervised_Auto-Labeling_via_Cycle-Consistency_ICCV_2021_paper.html
---

Our Paper: <a href= 'https://openaccess.thecvf.com/content/ICCV2021/html/Ganeshan_Warp-Refine_Propagation_Semi-Supervised_Auto-Labeling_via_Cycle-Consistency_ICCV_2021_paper.html'>"Warp-Refine Propagation: Semi-Supervised Auto-Labeling via Cycle-Consistency"</a> will be presented at IEEE/CVF International Conference on Computer Vision (ICCV), 2021 (<a href="https://iccv2021.thecvf.com/home"> ICCV-2021</a>)! I received great mentorship from my co-authors from Toyota Research Institute (<a href="https://adriengaidon.com/"> Adrien Gaidon</a>, <a href="https://scholar.google.se/citations?user=2xjjS3oAAAAJ&hl=en"> Rares Ambrus</a>, and <a href="https://scholar.google.com/citations?user=_UJsz3AAAAAJ&hl=en"> Dennis Park</a>) and from Preferred Networks (<a href="https://scholar.google.ca/citations?hl=en&user=Fv-ifUQAAAAJ&view_op=list_works&sortby=pubdate"> Shin-ichi Maeda</a>, and <a href="https://scholar.google.co.jp/citations?user=6g9DurAAAAAJ&hl=en"> Tommi Kerola</a>)!

## H2 Abstract:

{{ page.abstract }}