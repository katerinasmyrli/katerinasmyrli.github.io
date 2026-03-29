---
layout: page
title: Human mesh generation
description: Improving pose detection and automating gait phase identification
img: assets/img/humanoids_thumbnail.png
importance: 3
category: biomechanics
tags: [Biomechanics, Gait Analysis, Computer Vision, Robotics]
related_publications: true
---

> In this work we explore methods to improve the fidelity of markerless motion capture for gait analysis, combining insights from multi-view geometry, deep learning, and biomechanics.


<div class="row">
    <div class="col-md-7">
        <p>
        Our early work investigated the use of monocular pose estimation to extract biomechanical parameters such as limb lengths and joint configurations from simple RGB inputs. Even with minimal setup, we observed that meaningful gait descriptors can be recovered with reasonable agreement to marker-based systems, highlighting the potential of low-cost, fast acquisition pipelines {% cite eccomas19 %}.
        </p>
        <p>
        Building on this, we introduced a trinocular reconstruction pipeline that fuses multiple synchronized views into a single, refined 3D human representation. By aligning and merging per-view meshes, we reduce occlusions and reconstruction artifacts, enabling more accurate estimation of gait phases, joint trajectories, and human–environment interaction {% cite icip23 %}.
        </p>
    </div>
    <div class="col-md-5 text-center">
        {% include figure.liquid 
            path="assets/img/econ_mesh.png"
            class="img-fluid rounded"
        %}
        <div class="caption">
         Human mesh generation using ECON {% cite icip23 %}.
        </div>
    </div>
</div>

<div class="row">
    <div class="col-md-6 text-center">
        {% include figure.liquid 
            path="assets/img/avatar_humanoids.png"
            class="img-fluid rounded"
        %}
        <div class="caption">
         A digital avatar is recorded in simulation by a dense set of virtual cameras, enabling a number of viewpoints that would not be feasible in real setups. The resulting images are used to reconstruct the 3D mesh, and reconstruction quality is evaluated across the gait cycle to deduce optimal camera placements for each instance.  {% cite humanoids24 %}.
        </div>
    </div>
    <div class="col-md-6">
        <p>
        More recent work focuses on improving reconstruction quality at the mesh level. We study how camera placement and viewpoint selection affect deep-learning-based mesh reconstruction, and propose a simulation-driven framework to optimize camera configurations. Combined with mesh refinement techniques (alignment, evaluation, and surface reconstruction), this leads to significantly improved geometric consistency, particularly in lower-limb regions critical for gait analysis. A major result of this work is the detection of gait phases through the analysis of foot–ground mesh interaction, using reconstructed meshes of the foot and the ground {% cite humanoids24 %}.
        </p>
    </div>
</div>

<div class="row">
    <div class="col-md-8">
Overall, these efforts contribute toward a unified pipeline for markerless motion capture that approaches the fidelity of traditional systems, while remaining low-cost, non-intrusive, and scalable. The ongoing direction is to integrate these components into a robust toolchain capable of reliable 3D motion reconstruction and biomechanical analysis in unconstrained environments.
    </div>
    <div class="col-md-4 text-center">
        {% include figure.liquid 
            path="assets/img/footprint_humanoids.png"
            class="img-fluid rounded"
        %}
        <div class="caption">
         Left footprint estimated and used to detect contact events {% cite humanoids24 %}.
        </div>
    </div>
</div>

