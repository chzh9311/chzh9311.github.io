---
title: "Force-Aware 3D Contact Modeling for Stable Grasp Generation"
collection: publications
category: conferences
header:
  teaser: fagrasp-aaai-teaser.png
permalink: /publication/2026-fagrasp
excerpt:
date: 2026-01-21
venue: 'Annual AAAI Conference on Artificial Intelligence'
authors: 'Zhuo Chen, Zhongqun Zhang, Yihua Cheng, Ales Leonardis, Hyung Jin Chang'
webpageurl: 'https://chzh9311.github.io/force-aware-grasp-project'
paperurl: 'https://arxiv.org/abs/2511.13247'
citation: 'Chen Z, Zhang Z, Cheng Y, et al. Force-Aware 3D Contact Modeling for Stable Grasp Generation[C]. Annual AAAI Conference on Artificial Intelligence (AAAI), 2026.'
---

Contact-based grasp generation plays a crucial role in various applications. Recent methods typically focus on the geometric structure of objects, producing grasps with diverse hand poses and plausible contact points. However, these approaches often overlook the physical attributes of the grasp, specifically the contact force, leading to reduced stability of the grasp. In this paper, we focus on stable grasp generation using explicit contact force predictions. First, we define a force-aware contact representation by transforming the normal force value into discrete levels and encoding it using a one-hot vector. Next, we introduce force-aware stability constraints. We define the stability problem as an acceleration minimization task and explicitly relate stability with contact geometry by formulating the underlying physical constraints. Finally, we present a pose optimizer that systematically integrates our contact representation and stability constraints to enable stable grasp generation. We show that these constraints can help identify key contact points for stability which provide effective initialization and guidance for optimization towards a stable grasp. Experiments are carried out on two public benchmarks, showing that our method brings about 20% improvement in stability metrics and adapts well to novel objects.
