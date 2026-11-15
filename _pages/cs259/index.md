---
title: "CS 259: Architecture and Systems for Neural Rendering"
permalink: /teaching/cs259/
---

<img class="course-banner" src="{{ '/images/teaching/cs259/neural-rendering.jpg' | relative_url }}" alt="A 3D scene is encoded as a neural representation (an MLP neural field or 3D Gaussians), rendered on the GPU by ray marching or splatting on streaming multiprocessors, tensor cores, and HBM, and produces the final image.">
<p class="course-caption">Labs and projects use <a href="https://github.com/vortexgpgpu/vortex">Vortex</a>, a full-stack open-source GPU you can read, modify, and measure end to end.</p>

How does a GPU turn a scene into pixels, and what changes when part of the renderer is a neural network? This graduate course follows the rendering stack down into the hardware. We start with the GPU programming and execution model and core GPU microarchitecture, then study the graphics pipeline (rasterization, interpolation, texture sampling, and pixel shading) and ray-tracing hardware. The second half turns to neural rendering: how deep-learning super sampling and neural scene representations run on GPUs, and how tensor units, sparsity, and compression make them faster.

You will build these ideas hands-on with Vortex, which includes synthesizable RTL, a cycle-level simulator, a kernel compiler, and a runtime.

## Logistics

<dl class="course-facts">
  <dt>Instructor</dt>
  <dd><a href="{{ '/' | relative_url }}">Blaise-Pascal Tine</a> · blaisetine [at] cs.ucla.edu</dd>
  <dt>Current offering</dt>
  <dd>Lecture times, office hours, exam dates, and the discussion forum are posted in BruinLearn each term.</dd>
  <dt>Syllabus</dt>
  <dd><a href="{{ '/teaching/cs259/syllabus/' | relative_url }}">On this site</a> and in BruinLearn</dd>
</dl>

## What you will learn

- **GPU programming models:** CUDA and OpenCL for compute, and Vulkan and OpenGL for graphics.
- **Core GPU microarchitecture:** kernel scheduling, shared memory, and control-flow divergence.
- **Graphics pipeline microarchitecture:** rasterization, interpolation, texture sampling, and pixel shading.
- **Ray-tracing and tensor-unit microarchitecture.**
- **Accelerating neural graphics:** deep-learning super sampling and neural rendering on GPUs.

## Prerequisites

Background in computer architecture and hardware design is strongly recommended. If you need a PTE number to enroll, email the instructor; priority goes to students with hardware design and computer architecture background.

## Textbooks

- Tor M. Aamodt, Wilson Wai Lun Fung, and Timothy G. Rogers, *General-Purpose Graphics Processor Architecture*, Morgan & Claypool.
- David B. Kirk and Wen-mei W. Hwu, *Programming Massively Parallel Processors: A Hands-on Approach*, Morgan Kaufmann.
- Eric Haines and Tomas Akenine-Möller (editors), *Ray Tracing Gems*, Apress.

Readings also include conference papers and patents. Class notes are provided.
