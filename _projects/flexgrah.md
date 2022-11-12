---
title: "Flexgraph - A Reconfigurable Hybrid CPU-FPGA Graph Analytics Accelerator"
collection: project
type: "open-source"
pageurl: "https://github.com/gtcasl/flexgraph"
date: 2017-01-01
---

Flexgraph is a reconfigurable domain-specific accelerator for graph analytics targeting heteregenous CPU-FPGA platforms.

FlexGraph uses a Doubly Compressed Sparse Matrix format to eliminate unnecessary data transfers and reduce storage requirements. Our architecture allows support for other compressed format by decoupling the matrix data structure traversal from the compute and memory units. We introduce memory access hardware primitives for unstructured fine-grained accesses on cache-coherent shared memory. Flexgraph uses a C++ Hardware Generation Language to extend its vertex programming model with domain centric reconfigurability in an integrated single source development environment, providing a design efficient alternative to High Level Synthesis.