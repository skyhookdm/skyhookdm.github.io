---
title: Query processing for a computational storage system
subtitle: "[Computational I/O Stack Workshop, August 17, 2023](/post/20230718-aug17/)"
date: 2023-08-16
authors: [aldrin.montana]
image:
  focal_point: 'top'
---

Existing research in computational storage primarily explores pushdown of a single query
operator or its supporting functions from a database management system. In these cases,
the portion of a query that can be pushed down is static, the execution of the kernel is
device-specific, and the benefits of computational storage only exist between the database
system and the compuational storage devices (CS devices) it is directly connected to.
However, an optimal, static partitioning is likely to change whenever workload
characteristics shift, for varying device characteristics, and for evolving
characteristics of the storage system.

A storage system grows when new, heterogeneous storage devices are added to the storage
hierarchy. As characteristics of these devices evolve and they gain more compute
resources, it will be desirable (and necessary) to deploy heterogeneous data processing
and storage engines that are well designed for device-specific characteristics or
data-specific modeling and storage. I call a storage system designed for this complexity a
computational storage system (CS system).

We are working towards dynamic, just-in-time partitioning of computation to utilize the
extra compute resources available in a CS system. In this talk, I will describe how we
approach just-in-time partitioning of computation by decomposing a logical query plan
(initial query plan) into portions (subplans) that can be distributed. On any given CS
device, a subplan is processed locally, translated to a physical query plan, then the
physical query plan is executed. Execution of the physical query plan may be partial
(best-effort), and the portions that were not executed are propagated with the query
results so that CS devices higher in the data access path may, collectively, eventually
complete execution of the initial query plan.
