---
title: An HPC-Oriented Runtime Environment for Enabling Computational Storage
subtitle: "[Computational I/O Stack Workshop, August 17, 2023](/post/20230718-aug17/)"
date: 2023-08-11
authors: [matthew.curry]
image:
  focal_point: 'top'
---

There are at least two methods for enabling computational storage workflows on embedded storage hardware. The first revolutionary path is to port applications to relatively lightweight storage abstractions that allow simple software stacks. A second evolutionary path is to enable existing storage abstractions by porting existing libraries and utilities to computational storage hardware. While the evolutionary path is a good stop-gap measure until applications can be prepared, porting significant dependency chains for complex libraries to the required interesting architectures can be a significant hurdle.  
 
In this talk, I will describe the Advanced Tri-lab Software Environment (ATSE). ATSE is a traditional HPC software stack for testbed systems. As a full-featured stack, it is able to provide complex I/O libraries such as HDF5, NetCDF, CGNS, Exodus, and others. Crucially, ATSE has been demonstrated to port to many variants of Arm and RISC-V processors, allowing use on low-power hardware often found in computational storage devices. Along with the stack itself, this talk will touch on techniques and facilities allowing ATSE’s high levels of portability.
