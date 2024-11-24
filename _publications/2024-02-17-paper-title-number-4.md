---
title: "Joint-Limb Compound Triangulation With Co-Fixing for Stereoscopic Human Pose Estimation"
collection: publications
category: manuscripts
permalink: /publication/2024-CTCF
excerpt: 
date: 2024-06-06
venue: 'IEEE Transactions on Multimedia'
paperurl: 'http://chzh9311.github.io/files/TMM.pdf'
citation: 'Z. Chen, X. Wan, Y. Bao and X. Zhao, "Joint-Limb Compound Triangulation With Co-Fixing for Stereoscopic Human Pose Estimation," in IEEE Transactions on Multimedia, doi: 10.1109/TMM.2024.3410514. keywords: {Three-dimensional displays;Estimation;Pose estimation;Compounds;Stereo image processing;Feature extraction;Vectors;human pose estimation;triangulation;machine learning},'
---

As a special subset of multi-view settings for 3D human pose estimation, stereoscopic settings show promising applications in practice since they are not ill-posed but could be as mobile as monocular ones. However, when there are only two views, the problems of occlusions and “double counting” (ambiguity between symmetric joints) pose greater challenges that are not addressed by previous approaches. On this concern, we propose a novel framework to detect limb orientations in field form and incorporate them explicitly with joint features. Two modules are proposed to realize the fusion. At 3D level, we design compound triangulation as an explicit module that produces the optimal pose using 2D joint locations and limb orientations. The module is derived from reformulating triangulation in 3D space, and expanding it with the optimization of limb orientations. At 2D level, we propose a parameter-free module named co-fixing to enable joint and limb features to fix each other to alleviate the impact of “double counting”. Features from both parts are first used to infer each other via simple convolutions and then fixed by the inferred ones respectively. We test our method on two public benchmarks, Human3.6 M and Total Capture, and our method achieves state-of-the-art performance on stereoscopic settings and comparable results on common 4-view benchmarks.
