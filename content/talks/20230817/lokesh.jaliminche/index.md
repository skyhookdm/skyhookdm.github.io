---
title:  A Methodology to Assist Kernel Offloading Decisions on Computational Storage
subtitle: "[Computational I/O Stack Workshop, August 17, 2023](/event/20230817/)"
date: 2023-08-11
authors: [lokesh.jaliminche]
image:
  focal_point: 'top'
---

We have seen significant growth in data and data processing applications in recent years. For such applications, data movement has been one of the primary bottlenecks for performance and Energy consumption. Computational Storage Devices(CSDs) possess the potential to reduce data movement overheads by processing data in or near storage devices. However, we observe that their adaption has been slow because of the manual effort involved in analyzing applications to identify kernels that can be offloaded to CSDs. Existing methodologies follow an iterative implementation and evaluation cycle, which leads to a very slow design process and expensive iterations. In this talk, I will discuss our proposed methodology for application analysis and kernel identification with initial evaluation. 
