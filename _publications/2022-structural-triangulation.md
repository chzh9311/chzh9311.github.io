---
title: "Structural Triangulation: A Closed-Form Solution to Constrained 3D Human Pose Estimation"
collection: publications
category: conferences
permalink: /publication/2022-structral-triangulation
excerpt: 
date: 2022-11-06
venue: 'Computer Vision - ECCV 2022'
slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'http://academicpages.github.io/files/ECCV22.pdf'
citation: 'Chen, Z., Zhao, X., Wan, X. (2022). Structural Triangulation: A Closed-Form Solution to Constrained 3D Human Pose Estimation. In: Avidan, S., Brostow, G., Cissé, M., Farinella, G.M., Hassner, T. (eds) Computer Vision – ECCV 2022. ECCV 2022. Lecture Notes in Computer Science, vol 13665. Springer, Cham. https://doi.org/10.1007/978-3-031-20065-6_40'
---

We propose Structural Triangulation, a closed-form solution for optimal 3D human pose considering multi-view 2D pose estimations, calibrated camera parameters, and bone lengths. To start with, we focus on embedding structural constraints of human body in the process of 2D-to-3D inference using triangulation. Assume bone lengths are known in prior, then the inference process is formulated as a constrained optimization problem. By proper approximation, the closed-form solution to this problem is achieved. Further, we generalize our method with Step Constraint Algorithm to help converge when large error occurs in 2D estimations. In experiment, public datasets (Human3.6M and Total Capture) and synthesized data are used for evaluation. Our method achieves state-of-the-art results on Human3.6M Dataset when bone lengths are known and competitive results when they are not. The generality and efficiency of our method are also demonstrated.
