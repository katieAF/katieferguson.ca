---
layout: page
title: research
permalink: /projects/
description:
nav: true
nav_order: 2
display_categories: [current research]
horizontal: true
tabs: true
---

{% tabs research %}

{% tab research approaches %}

<p class="mt-3">I study how the brain shapes what we perceive. Combining imaging, electrophysiology, targeted manipulations, and behavior in mice with computational modeling and quantitative analysis, I dissect how specific cell types in cortical circuits give rise to flexible, context-dependent perception.</p>

<h2 class="approach-group">Systems</h2>

<div class="card mt-3 p-3">
  <h5 class="font-weight-bold">Optical Imaging</h5>
  <div class="row align-items-center">
    <div class="col-md-4 mb-3 mb-md-0">
      {% include figure.liquid loading="eager" path="assets/img/PN.gif" title="Two-photon calcium imaging" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-md-8">
      <p class="mb-0" style="font-size: 0.95em;">Recordings of neural activity in awake, behaving mice using two-photon calcium imaging to track hundreds of individual neurons during visual tasks, and one-photon mesoscale imaging to capture activity across cortical areas. Intersectional genetic tools allow simultaneous monitoring of distinct cell populations, for example SST and VIP interneurons in the same field of view.</p>
    </div>
  </div>
</div>

<div class="card mt-3 p-3">
  <h5 class="font-weight-bold">Electrophysiology</h5>
  <div class="row align-items-center">
    <div class="col-md-4 mb-3 mb-md-0">
      {% include video.liquid path="assets/img/raster_animation.mp4" class="img-fluid rounded z-depth-1" autoplay=true loop=true muted=true controls=true cache_bust=true %}
    </div>
    <div class="col-md-8">
      <p class="mb-0" style="font-size: 0.95em;">High-density extracellular recordings using Neuropixels probes for fast, deep, multi-region access to neural activity. Complementary to imaging, trading cell-type identity for temporal resolution and depth coverage. A growing direction in my work.</p>
    </div>
  </div>
</div>

<div class="card mt-3 p-3">
  <h5 class="font-weight-bold">Circuit Manipulation</h5>
  <div class="row align-items-center">
    <div class="col-md-4 mb-3 mb-md-0">
      {% include figure.liquid loading="eager" path="assets/img/opto_mouse_schematic.png" title="Optogenetic manipulation schematic" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-md-8">
      <p class="mb-0" style="font-size: 0.95em;">Causally testing how specific cell types contribute to visual processing and behavior, primarily through optogenetic targeting of genetically defined populations, alongside chemogenetic and pharmacological approaches. Used in combination with both imaging and electrophysiology to link manipulation to circuit-level and population-level effects.</p>
    </div>
  </div>
</div>

<h2 class="approach-group">Behavior</h2>

<div class="card mt-3 p-3">
  <h5 class="font-weight-bold">Behavior</h5>
  <div class="row align-items-center">
    <div class="col-md-4 mb-3 mb-md-0">
      {% include video.liquid path="assets/img/behavior_video_22509_labeled_with_paradigm.mp4" class="img-fluid rounded z-depth-1" autoplay=true loop=true muted=true controls=true cache_bust=true %}
    </div>
    <div class="col-md-8">
      <p class="mb-0" style="font-size: 0.95em;">Designing and running visual detection and discrimination tasks in head-fixed mice, including task design, training, hardware integration, and the quantitative analysis that links neural activity to perceptual performance. Behavior is treated as a full experimental program, not a downstream readout.</p>
    </div>
  </div>
</div>

<h2 class="approach-group">Computational</h2>

<div class="card mt-3 p-3">
  <h5 class="font-weight-bold">Computational Modeling</h5>
  <p class="mb-0" style="font-size: 0.95em;">Biophysically grounded network models constrained by experimental data, used to test mechanistic hypotheses about how circuit properties give rise to neural dynamics and behavior. Builds on PhD work modeling hippocampal interneuron circuits.</p>
</div>

<div class="card mt-3 p-3">
  <h5 class="font-weight-bold">Quantitative Methods</h5>
  <p class="mb-0" style="font-size: 0.95em;">Statistical and machine learning approaches for large-scale neural data, including dimensionality reduction, neural manifold analysis, GLMs, mixed-effects models, and population-level decoding. Connects experimental work back to the analytical framing that drives interpretation.</p>
</div>

{% endtab %}

{% tab research projects %}

<div class="projects mt-3">
{% assign sorted_projects = site.projects | sort: "importance" %}

<div class="container">
  <div class="row row-cols-1">
  {% for project in sorted_projects %}
    {% include projects_horizontal.liquid %}
  {% endfor %}
  </div>
</div>
</div>

{% endtab %}

{% endtabs %}
