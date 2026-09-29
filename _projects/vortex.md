---
title: "Vortex - Open-Source RISC-V GPU"
collection: project
type: "open-source"
pageurl: "https://vortexgpgpu.github.io/"
date: 2021-01-01
excerpt: "A full-stack, open-source RISC-V GPU: hardware (RTL), compiler and runtime, and a graphics and compute software stack. Used by research groups worldwide."
---

Vortex is a full-stack, open-source RISC-V GPU. It spans the hardware (RTL) of a multicore GPU pipeline optimized for FPGAs, a compiler and runtime toolchain, a graphics and compute software stack, and a cycle-level simulator for design-space exploration.

Vortex has grown to cover high-bandwidth memory and graphics, the RISC-V vector ISA and its compiler, tensor-core AI architectures, and ray tracing. See [Research](/research/) for the work behind each step. Source code: [github.com/vortexgpgpu/vortex](https://github.com/vortexgpgpu/vortex).

## Built on Vortex

Vortex has become a reference platform for GPU architecture research. The following work by other groups uses Vortex as its hardware or software platform.

### Top-tier architecture venues

* M. Zerva, P.-E. Eleftherakis, A. Maras, K. Iliakis, A. Moiras, and S. Xydis (NTUA), "sCROOGe: Circuit-level Design and Optimization Framework for RISC-V Out-of-Order GPUs," ISCA, 2026.
* H. Kim, R. R. Yan, J. You, T. V. Yang, and Y. S. Shao (UC Berkeley), "Virgo: Cluster-level Matrix Unit Integration in GPUs for Scalability and Energy Efficiency," ASPLOS, 2025.
* A. Nada, G. M. Sarda, and E. Lenormand, "Cooperative Warp Execution in Tensor Core for RISC-V GPGPU," HPCA, 2025.
* S. Jeong, L. P. Cooper, J. M. Lee, H. Choi, N. Parnenzini, C. Ahn, Y. Lee, H. Kim, and H. Kim (Georgia Tech), "SparseWeaver: Converting Sparse Operations as Dense Operations on GPUs for Graph Workloads," HPCA, 2025.
* Y. Zhang, M. Wang, W. Wang, Y. Mai, H. Huang, and Z. Yu, "Atomic Cache: Enabling Efficient Fine-Grained Synchronization with Relaxed Memory Consistency on GPGPUs Through In-Cache Atomic Operations," MICRO, 2024.
* F. Elsabbagh, S. Sheikhha, V. A. Ying, Q. M. Nguyen, J. S. Emer, and D. Sanchez (MIT), "Accelerating RTL Simulation with Hardware-Software Co-Design," MICRO, 2023.

### Other venues

* S. Machetti, P. D. Schiavone, L. Orlandic, D. Huang, D. Kasap, G. Ansaloni, and D. Atienza (EPFL), "e-GPU: An Open-Source and Configurable RISC-V GPU for TinyAI Applications," arXiv, 2025.
* M. Solé i Bonet, J. Wolf, L. Kosmidis, et al. (BSC / UPC), METASAT platform series: "The METASAT Hardware Platform" (EDHPC, 2023); "A RISC-V Multicore and GPU SoC Platform with a Qualifiable Software Stack for Safety-Critical Systems" (DATE, 2025); "A Qualifiable GPU Sharing Approach for AI Workloads in Critical Systems" (HPEC, 2025); "Integration of GPU RTL IP into System-Level Simulation through TLM" (Software Engineering Companion, 2025); and a METASAT/XtratuM follow-on (Microprocessors & Microsystems, vol. 121, 2026).
* D. Gouk, S. Kang, S. Lee, et al., "CXL-GPU: Pushing GPU Memory Boundaries with the Integration of CXL Technologies," IEEE Micro, vol. 45, no. 6, 2025.
* N. Crouzet, T. Carle, and C. Rochange, "Time-Predictable Warp Scheduling in a GPU," Microprocessors & Microsystems, vol. 118, 2025.
* Y. Cheng, Y. Man, and X. Zhou, "A High-Performance Branch Control Mechanism for GPGPU Based on RISC-V Architecture," Electronics, vol. 15, no. 1, 2026.
* S. Magalhães, P. Oliveira, and R. Marks, "Implementation and Evaluation of Warp-Scheduling Policies in Vortex, an Open-Source GPGPU," SSCAD, 2025.
* G. M. Sarda, N. Shah, D. Bhattacharjee, P. Debacker, and M. Verhelst, "Optimising GPGPU Execution Through Runtime Micro-Architecture Parameter Analysis," IISWC, 2023.
* S. Chetput, A. Nallathambi, et al., "Integrating RISC-V SIMT and Scalar Cores: Loosely to Tightly Coupled," RISC-V for HPC Workshop @ ISC High Performance, 2024.
* Z. Jiang, K. Zheng, Y. Bao, and K. Shi (ICT/CAS), "Verification Framework for RISC-V with Custom Instruction Extensions," ISEDA, 2024.
* G. M. Sarda, N. Shah, A. Nada, D. Bhattacharjee, and M. Verhelst, "Decoupled Control Flow and Data Access in RISC-V GPGPUs," arXiv, 2025.
* W. Matsumi and R.-U.-H. Mian, "Accelerating HDC-CNN Hybrid Models Using Custom Instructions on RISC-V GPUs," arXiv, 2025.
* R. R. Yan (UC Berkeley), "SonicSim: Socket-based Hardware Co-Simulation with Inter-Process Communication," UC Berkeley EECS Technical Report, 2024.
* D. Million, C. Fuguet, and A. Evans (CEA), "Preliminary Integration of Vortex within the OpenPiton Platform," Vortex Workshop @ MICRO, 2024.
