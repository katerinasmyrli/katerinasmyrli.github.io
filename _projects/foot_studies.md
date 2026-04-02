---
layout: page
title: Foot shape investigations
description: From circular to custom foot geometry
img: assets/img/footshape.png
importance: 3
category: bipedal gait
tags: [Biomechanics, Gait Analysis, Computer Vision, Robotics]
related_publications: true
---

> This project explores how foot geometry fundamentally shapes passive walking dynamics. Starting from simple circular feet, we progressively moved toward more expressive representations: elliptical and finally arbitrary geometries that better capture human-like gait and unlock new design possibilities for robotics and prosthetics.

Early work in passive bipedal walking relied heavily on circular feet due to their analytical simplicity. Circular feet produce a simple rolling motion, and their radius directly influences gait characteristics such as speed and stability. However, this simplicity comes at a cost: the human foot does not behave as a constant-radius rocker, limiting the ability of circular models to reproduce realistic human gait patterns. {% cite smyrli21 %}

<div class="row">
    <div class="col-md-7 text-center">
      {% include figure.liquid 
            path="assets/img/elliptic_feet.png"
            class="img-fluid rounded"
        %}
        <div class="caption">
          Effects of varying rolling curvature profiles in foot shapes during bipedal walking. {% cite iros19 %}.
        </div>
    </div>
    <div class="col-md-5">
        To bridge this gap, we introduced semi-elliptical feet in a collaboration between NTUA and the University of Duisburg-Essen. Unlike circles, elliptical geometries provide a varying curvature during stance, allowing the rolling radius to change throughout the step. This better approximates the human rollover behavior, where curvature is lower at heel-strike and toe-off and higher when the foot is flat. 
Through this model, we showed how foot shape curvature variation significantly affects gait characteristics such as stability, walking speed, and impact forces, and that properly tuned curvature can improve energetic efficiency for a target walking speed. {% cite iros19 %}
    </div>
</div>

<div class="row">
    <div class="col-md-8">
      <p>
        However, even elliptical feet impose strong geometric constraints. They only allow a limited range of shapes and therefore restrict the achievable ankle trajectories. Human walking, in contrast, emerges from a complex multi-joint foot that cannot be accurately captured by a single parametric curve.
      </p>
      <p>
To overcome this limitation, we developed a generalized framework that allows analytical description of passive walking dynamics with arbitrary convex foot shapes, defined simply as a set of points. 
This formulation decouples body dynamics from foot-ground interactions and enables the incorporation of any geometry into the gait model, without requiring a closed-form analytical description.
      </p>
      <p>
Using this framework, we designed foot shapes directly from human data. By estimating human ankle trajectories using a markerless motion capture system, we identified foot geometries that reproduce human-like motion through purely passive dynamics. 
This represents a shift from <i>assuming</i> foot geometry to <i>designing it for a desired gait outcome</i>. {% cite icra20 %}
      </p>
      <p>
The key result is that foot shape is not just a modeling choice: it is a powerful design variable. By moving from circular to arbitrary geometries, we enable precise control of ankle trajectories, improved energetic performance, and personalized foot design for robotics and prosthetics.
      </p>
    </div>
    <div class="col-md-4 text-center">
        {% include figure.liquid 
            path="assets/img/foot_shape.png"
            class="img-fluid rounded"
        %}
        <div class="caption">
          (a-f) Selected frames from OpenPose output for step video
sequence. Stance leg in cyan, swing leg in blue. Ankle trajectory in red. {% cite icra20 %}.
        </div>
        {% include figure.liquid 
            path="assets/img/foot_shape2.png"
            class="img-fluid rounded"
        %}
        <div class="caption">
            (a) Points defining the foot shape. (b) Biped ankle trajectory for
full and partial rotation, compared to experimental data from OpenPose.  {% cite icra20 %}.
        </div>
    </div>
</div>



Ultimately, this progression transforms foot design from a single parameter selection into an unbounded optimization space, opening the door to data-driven and task-specific design of locomotion systems.
