---
layout: page
title: Foot shape investigations
description: From circular to arbitrary foot heometry
img: assets/img/humanoids_thumbnail.png
importance: 3
category: bipedal gait
tags: [Biomechanics, Gait Analysis, Computer Vision, Robotics]
related_publications: true
---

This project explores how foot geometry fundamentally shapes passive walking dynamics. Starting from simple circular feet, we progressively moved toward more expressive representations—elliptical and finally arbitrary geometries—to better capture human-like gait and unlock new design possibilities for robotics and prosthetics.

Early work in passive bipedal walking relied heavily on circular feet due to their analytical simplicity. Circular feet produce stable and predictable rolling motion, and their radius directly influences gait characteristics such as speed and stability. However, this simplicity comes at a cost: the human foot does not behave as a constant-radius rocker, limiting the ability of circular models to reproduce realistic gait patterns. :contentReference[oaicite:0]{index=0}

To bridge this gap, we introduced semi-elliptical feet. Unlike circles, elliptical geometries provide a varying curvature during stance, allowing the rolling radius to change throughout the step. This better approximates the human rollover behavior, where curvature is lower at heel-strike and toe-off and higher when the foot is flat. :contentReference[oaicite:1]{index=1}  
Through this model, we showed that foot shape significantly affects gait characteristics such as stability, walking speed, and impact forces, and that properly tuned curvature can improve energetic efficiency for a target walking speed. :contentReference[oaicite:2]{index=2}

However, even elliptical feet impose strong geometric constraints. They only allow a limited range of shapes and therefore restrict the achievable ankle trajectories. Human walking, in contrast, emerges from a complex multi-joint foot that cannot be accurately captured by a single parametric curve.

To overcome this limitation, we developed a generalized framework that allows passive walking simulation with arbitrary convex foot shapes, defined simply as a set of points. :contentReference[oaicite:3]{index=3}  
This formulation decouples body dynamics from foot-ground interaction and enables the incorporation of any geometry into the gait model, without requiring a closed-form analytical description.

Using this framework, we designed foot shapes directly from data. By estimating human ankle trajectories using OpenPose, we identified foot geometries that reproduce human-like motion through purely passive dynamics. :contentReference[oaicite:4]{index=4}  
This represents a shift from *assuming* foot geometry to *designing it for a desired gait outcome*.

The key result is that foot shape is not just a modeling choice—it is a powerful design variable. By moving from circular to arbitrary geometries, we enable:
- precise control of ankle trajectories,
- improved energetic performance,
- and personalized foot design for robotics and prosthetics.

Ultimately, this progression transforms foot design from a constraint into an optimization space, opening the door to data-driven and task-specific locomotion systems.
