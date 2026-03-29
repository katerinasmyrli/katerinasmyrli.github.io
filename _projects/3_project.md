---
layout: page
title: project 3 with very long name
description: a project that redirects to another website
img: assets/img/7.jpg
importance: 3
category: biomechanics
tags: [Biomechanics, Gait Analysis, Computer Vision, Robotics]
related_publications: true
---

> In this project we develop a low-cost gait analysis system that removes the need for traditional motion-capture labs. Instead of relying on markers and force plates, we use a stereo RGB camera and a simplified 2D biomechanical model to estimate human motion and dynamics.

At its core, the system combines computer vision with biomechanics. A markerless pose estimation pipeline extracts key body points, which are then used to reconstruct joint motion through inverse kinematics. Building on this, inverse dynamics allows the estimation of internal joint torques and ground reaction forces—all without specialized equipment.

The model is designed in the sagittal plane with 14 degrees of freedom, balancing simplicity and physical accuracy. A key contribution is the ability to recover dynamic quantities typically requiring force plates, making the system portable, affordable, and fast to deploy.

Our work demonstrates that meaningful gait analysis can be performed outside specialized labs, opening the door to applications in rehabilitation, sports analysis, and human-robot interaction.

Results of this work have been published in {% cite bibe25 %}.
