---
layout: page
title: PhD thesis
description: with background image
img: assets/img/prosth_des.png
importance: 1
category: bipedal gait
related_publications: true
---

    This thesis investigates the dynamics of bipedal locomotion through the modeling, simulation, and control of passive and active bio-inspired mechanical walkers, with emphasis on applications in robotics and lower-limb prosthetics. 

The research follows a structured progression, beginning with a bipedal walking _base_ model that captures key aspects of human walking using compliant legs and semicircular feet. Despite its simplicity, this initial model exhibits stable passive walking cycles that resemble human gait. A nondimensional formulation enables sensitivity analysis, fixed-point identification, and energetic evaluation across a wide range of design parameters. The model's predictions are validated through multibody simulations using a digital twin and through the development and use of an experimental prototype.

Building on this foundation, the design of the model is gradually refined to incorporate more anatomically inspired features. The study advances through a series of _footshape investigations_, beginning with a semielliptical design that approximates the evolving curvature of the human foot during rollover. This model allows a parametric investigation of rollover dynamics, allowing the fine-tuning of gait descriptors and the optimization of energetic efficiency. The model is subsequently expanded to support any convex foot geometry, enabling the integration of biomimetic profiles extracted from experimental human walking data. These geometries allow the replication of biomimetic ankle trajectories and prediction of ground contact behavior with increasing fidelity, offering a clear pathway for prosthetic foot design that mirrors natural biomechanics.

The work continues through the study of _knee joint morphology_. An initial passive kneed model is developed that uses simple pin joints. Passive gaits for this walker are identified, and the effect of parameter variations is investigated. The model is later compared with a novel biomimetic four-bar kneed model, inspired by the human cruciate ligament system. The four-bar configuration exhibits superior compliance, impact absorption and energetic efficiency, which are critical for the design of functional prosthetic knees. Comparative simulations reveal the importance of joint design in achieving both gait stability and energetic performance.

To extend these passive behaviors to level-ground locomotion, a novel Underactuated Virtual Gravity control framework is introduced. This controller analytically replicates the gravitational torques experienced during downhill passive walking, enabling highly efficient locomotion with minimal actuation. Implemented on a bipedal robot model that features a counterweight torso, the UVG control scheme achieves dynamic behaviors closely aligned with the passive model, while requiring low motor effort, offering strong potential for integration into active prosthetic systems. Moreover, the UVG control output is compared to an alternative actuation approach based on trajectory optimization and stabilization. The UVG is found to outperform the alternative scheme, due to its passive dynamics-based approach.

In parallel, a markerless, stereo-camera-based gait analysis system is developed to extract full-body kinematic and kinetic data from _human walking_ trials. Using neural network-based pose estimation and inverse dynamics analysis, this system provides joint torque and ground reaction force estimates without requiring markers or force plates. These human gait data are used to inform and calibrate the robotic models, ensuring that the simulated behaviors converge to real human biomechanics. 

The outcome of this research is a comprehensive framework for bipedal walking analysis and robotic or prosthetic design. The combination of detailed modeling, parametric tuning and efficient control provides valuable tools for the development of lower-limb prostheses that closely emulate human motion. The work contributes to the understanding of energy-efficient gait generation, design-driven dynamics, and controller synthesis, offering new perspectives in both robotics and assistive device engineering.



    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
