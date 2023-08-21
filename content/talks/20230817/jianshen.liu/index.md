---
title: Opportunistic Query Execution on SmartNICs for Analyzing In-Transit Data
subtitle: "[Computational I/O Stack Workshop, August 17, 2023](/post/20230718-aug17/)"
date: 2023-08-11
authors: [jianshen.liu]
url_slides: https://docs.google.com/presentation/d/1yt1s6fQ0ugHSJi9MxIbr4KkK3Gyns2J16hqX1Lj1hgY/edit#slide=id.g23baeb98e7b_0_253
image:
  focal_point: 'top'
---

High-performance computing (HPC) systems researchers have proposed using current, programmable network interface cards (or SmartNICs) to offload data management services that would otherwise consume host processor cycles in a platform. While this work has successfully mapped data pipelines to a collection of SmartNICs, users require a flexible means of inspecting in-transit data to assess the live state of the system. In this paper, we explore SmartNIC-driven opportunistic query execution, i.e., enabling the SmartNIC to make a decision about whether to execute a query operation locally (i.e., "offload") or defer execution to the client (i.e., "push-back"). Characterizations of different parts of the end-to-end query path allow the decision engine to make complexity predictions that would not be feasible by the client alone.