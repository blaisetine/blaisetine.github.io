---
title: "CS 254A: GPU Microarchitecture"
permalink: /cs254a/
---

<img class="course-banner" src="{{ '/images/teaching/cs254a/gpu-architecture.jpg' | relative_url }}" alt="A workload is compiled into a kernel that runs across many GPU streaming multiprocessors, each with tensor cores and ray-tracing units, backed by high-bandwidth memory (HBM).">
<p class="course-caption">Labs and projects use <a href="https://github.com/vortexgpgpu/vortex">Vortex</a>, a full-stack open-source GPU you can read, modify, and measure end to end.</p>

This graduate course takes you from the GPU programming model to the research frontier of GPU design. We start with how GPUs execute parallel programs (threads, warps, and memory models), then open up the hardware: instruction sets, core microarchitecture, divergence and warp scheduling, and the memory system. The second half covers scaling to many cores and chiplets, tensor-core architectures for AI, ray-tracing hardware for graphics, and emerging directions.

You will study these ideas hands-on with Vortex, which includes synthesizable RTL, a cycle-level simulator, a kernel compiler, and a runtime.

## Logistics

<dl class="course-facts">
  <dt>Instructor</dt>
  <dd><a href="{{ '/' | relative_url }}">Blaise-Pascal Tine</a> · blaisetine [at] cs.ucla.edu</dd>
  <dt>Current offering</dt>
  <dd>Lecture times, office hours, exam dates, and the discussion forum are posted in BruinLearn each term.</dd>
  <dt>Syllabus</dt>
  <dd><a href="{{ '/cs254a/syllabus/' | relative_url }}">On this site</a> and in BruinLearn</dd>
</dl>

## What you will learn

- **The GPGPU programming model:** CUDA and OpenCL programming.
- **Core GPU architecture:** execution and memory models, instruction sets, microarchitecture organization and implementation, and control-flow and scheduler optimizations.
- **Domain-specific acceleration:** machine learning and graphics rendering.

## Prerequisites

Background in computer architecture and hardware design (Verilog) is strongly recommended. If you need a PTE number to enroll, email the instructor; priority goes to students with hardware design and computer architecture background.

## Textbooks

- Tor M. Aamodt, Wilson Wai Lun Fung, and Timothy G. Rogers, *General-Purpose Graphics Processor Architecture*, Morgan & Claypool.
- David B. Kirk and Wen-mei W. Hwu, *Programming Massively Parallel Processors: A Hands-on Approach*, Morgan Kaufmann.

Readings also include conference papers and patents. Class notes are provided.
