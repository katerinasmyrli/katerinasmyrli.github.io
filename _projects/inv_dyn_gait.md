---
layout: page
title: Human gait analysis
description: inverse dynamics
img: assets/img/bibe_thumbnail.jpg
importance: 3
category: biomechanics
tags: [Biomechanics, Gait Analysis, Computer Vision, Robotics]
related_publications: true
---

> In this project we develop a low-cost gait analysis system that removes the need for traditional motion-capture labs. Instead of relying on markers and force plates, we use a stereo RGB camera and a simplified 2D biomechanical model to estimate human motion and dynamics.

At its core, the system combines computer vision with biomechanics. A markerless pose estimation pipeline extracts key body points, which are then used to reconstruct joint motion through inverse kinematics. Building on this, inverse dynamics allows the estimation of internal joint torques and ground reaction forces—all without specialized equipment.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/bibe_fig.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Simplified 2D model of the human body used in this study {% cite bibe25 %}.
</div>


The model is designed in the sagittal plane with 14 degrees of freedom, balancing simplicity and physical accuracy. A key contribution is the ability to recover dynamic quantities typically requiring force plates, making the system portable, affordable, and fast to deploy.

Our work demonstrates that meaningful gait analysis can be performed outside specialized labs, opening the door to applications in rehabilitation, sports analysis, and human-robot interaction.

Results of this work have been published in {% cite bibe25 %}.
