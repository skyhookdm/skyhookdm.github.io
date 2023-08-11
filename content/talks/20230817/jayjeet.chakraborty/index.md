---
title: Towards Faster Columnar Data Transport using RDMA
subtitle: "[Computational I/O Stack Workshop, August 17, 2023](/post/20230718-aug17/)"
date: 2023-08-11
authors: [jayjeet.chakraborty]
image:
  focal_point: 'top'
---

The amount of data stored in data centers worldwide is increasing faster than ever. Much of this data is stored to process, analyze, and extract valuable insights. Primarily, large datasets are stored in dumb storage servers inside data centers. To perform analysis and compute on this data, it must first be transported to compute servers, usually with big DRAMs and huge processing capabilities, where the data is processed and result sets sent to the client. Traditional data transport frameworks use TCP/IP as their underlying protocol and therefore require the users to provide with a single contiguous buffer for transfer to the framework. We observe that this approach adds a severe overhead when transferring batches of columnar records. Columnar tables consist of several buffers scattered in the memory, each representing a particular column and its metadata. Serializing these buffers into a single buffer requires doing multiple memory copies. To avoid this serialization overhead while transfer columnar batches over the wire, we propose using RDMA as a potential solution to this problem. In this paper, we explore transporting columnar result sets over RDMA from a server to a client and compare this approach with a state-of-the-art TCP/IP based transport framework. We show that using RDMA for columnar data transport provides up to 2x higher throughput. 