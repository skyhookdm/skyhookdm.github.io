---
title: "Split gRPC: An Isolation Architecture for RPC Stacks on SmartNICs"
subtitle: "[Computational I/O Stack Workshop, August 17, 2023](/post/20230718-aug17/)"
date: 2023-08-11
authors: [esteban.ramos]
url_slides: https://docs.google.com/presentation/d/18e9gYKn6ls_Tk79vXAEtqe3s7CU1zIkg5sjogCqU8z8/edit#slide=id.p
image:
  focal_point: 'top'
---

Remote procedure calls are a major contributor to performance variance in distributed systems due to lack of isolation and contention on shared resources. In this talk, I will introduce the novel architecture we built to address this problem, and cover our experience in implementing a prototype over gRPC with an emphasis on the communication layer between a host CPU and the SmartNIC. The basic idea is to partition RPC applications into two communicating components: one dedicated to user-implemented business logic, and one dedicated to RPC infrastructure processing. The infrastructure process can be run on a dedicated core or on a smart NIC (e.g., IPU or DPU), providing effective physical isolation and predictable performance. An evaluation of a proof-of-concept prototype shows that the split architecture adds modest overhead for average case latency, but allows for lower latency and and higher throughput under host CPU load.
