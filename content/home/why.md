---
widget: blank
headless: true
weight: 30
title: 🤔 Why Storage & Network Layers?
design:
  columns: "2"
  css_style: null
  css_class: null
---
A key challenge in data science is extracting efficient and timely insights from an ever increasing flood of data streams. Apache Arrow, an open source data processing framework, provides an efficient and timely approach by reducing in-memory serialization and copy overheads. It is widely used in the development of data management services of structured data due to its interoperability across multiple programming languages and runtimes and plays an essential role in the rapid evolution of the open source data science ecosystem. 

While many existing data management services that use Apache Arrow are well-suited for resource-rich environments, the open source data science ecosystem lacks a common framework for data management services designed for resource-constrained environments, like those found in the storage and networking layers. This has led to a variety of insular and hard-to-reuse embedded data processing solutions. An efficient approach is to reduce data movement within the storage and networking layers by embedding data reductive processing and caching throughout the data path. Like most emerging technologies, computational storage devices, smart NICs, and similar devices where data processing can be embedded have to overcome market entry barriers. Thus reducing complexity, increasing interoperability, and lower development costs are critical issues in embedded data management.

SkyhookDM is a full-stack data management framework with the purpose of bridging the gap between resource-rich and resource-constrained environments to better serve data-intensive applications. By leveraging Apache Arrow in the storage and networking layers, SkyhookDM adds extra data processing capabilities to embedded devices that were previously inflexible black boxes. This allows SkyhookDM to lower market entry barriers by saving costs and accelerating the development of data management services of structured data.

Beyond the integration and portability of data management services to embedded devices, SkyhookDM allows data management systems to interoperate with heterogeneous data management services, data sources, and devices in the storage and networking layers. Sharing rich metadata from data management systems to embedded devices allows data management services to become smarter and better adapt to heterogeneous architectures. This allows truly distributed data management services to interact even more intelligently with their specific hardware and software contexts.