---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

My research program is built around [Vortex](https://vortexgpgpu.github.io/), a full-stack, open-source RISC-V GPU. A credible open GPU platform is a prerequisite for reproducible architecture research, and for hands-on education that is not locked inside proprietary hardware. Vortex has since grown into each major domain of modern GPU architecture.

## Memory and graphics

We extended Vortex with high-bandwidth memory support to increase memory-level parallelism, and integrated a complete graphics hardware stack.

* [Skybox: Open-Source Graphic Rendering on Programmable RISC-V GPUs](/publications/asplos-23/) (ASPLOS 2023)
* [Towards "True" GPU Performance Scaling for OpenGPU](/publications/hotchips-24/) (Hot Chips 2024)
* [Analysis of the RISC-V Vector Extension for Vulkan Graphics Kernels](/publications/ispass-25-rvv-vulkan/) (ISPASS 2025)

## Vector ISA and compilers

We added RISC-V vector ISA support to the GPU and extended the compiler stack to target it, along with CUDA compatibility and fast performance modeling.

* [VESICA: Fused Vector Extension for RISC-V Embedded GPUs](/publications/iccad-26-vesica/) (ICCAD 2026)
* [Inside VOLT: Designing an Open-Source GPU Compiler](/publications/cc-26-volt/) (CC 2026)
* [SoftCUDA: Running CUDA on Softcore GPU](/publications/fccm-25-softcuda/) (FCCM 2025)
* [FastTrackGPU: Static-Analysis-Guided Analytical Modeling for Softcore GPUs](/publications/cal-26-fasttrackgpu/) (IEEE CAL 2026)

## Tensor AI and ray tracing

We broadened Vortex to support tensor-core architectures, structured and unstructured sparsity, and dedicated ray-tracing hardware.

* [PRISM: Accelerating Ray Tracing on RISC-V GPU](/publications/iccd-26-prism/) (ICCD 2026)
* Sparse tensor cores, 2:4 structured sparsity, microscaling formats, asynchronous barriers and TMA ([OSCAR 2026](/publications/#workshop-papers))
