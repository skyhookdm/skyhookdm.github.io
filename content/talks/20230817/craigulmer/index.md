---
title: Extending Composable Data Services into SmartNICs
subtitle: "[Computational I/O Stack Workshop, August 17, 2023](/post/20230718-aug17/)"
date: 2023-08-11
authors: [craigulmer]
url_slides: 230519_ulmer_compsys_smartnics_final.pdf
image:
  focal_point: 'top'
---

Advanced, scientific-computing workflows rely on composable data service libraries to migrate data between different simulation and analysis jobs that run in parallel on a high-performance computing (HPC) platform. While these services are essential for staging and transforming in-transit data, they consume compute node resources that could otherwise be used for scientific work. Recent programmable network interface cards (or SmartNICs) provide a new alternative for hosting services that enables data management tasks to run in an isolated space at the compute node that does not impact host resources. In this talk we explore extending composable data services into SmartNICs and describe a software stack for services that uses Faodel and Apache Arrow. To illustrate how this stack operates, we present a case study that implements a distributed, particle-sifting service for reorganizing simulation results. Performance experiments from a 100-node cluster equipped with 100Gb/s BlueField-2 SmartNICs indicate that current SmartNICs can perform useful data management tasks, albeit at a lower throughput than hosts.