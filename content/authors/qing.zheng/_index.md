---
# Display name
title: Qing Zheng

# Username (this should match the folder name)
authors:
- qing.zheng

# Is this the primary user of the site?
superuser: false

# Role/position
role: Assistant Computer Scientist, Los Alamos National Laboratory

# Organizations/Affiliations
organizations:
- name: LANL High Performance Computing (HPC) Division
  url: https://lanl.gov/org/ddste/aldsc/hpc/index.php
- name: Los Alamos National Laboratory
  url: https://lanl.gov/

# Short bio (displayed in user profile at end of posts)
bio: Qing Zheng is a Scientist in Los Alamos National Lab’s High-Performance Computing Division and a member of the Lab’s Ultrascale System Research Center. Qing performs I/O and storage research that guides the Lab’s future computing platform and storage infrastructure designs. Qing received his PhD in Computer Science from Carnegie Mellon University in 2021. 

# Social/Academic Networking
# For available icons, see: https://sourcethemes.com/academic/docs/widgets/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.
social:
- icon: envelope
  icon_pack: fas
  link: mailto:zhengqmark@gmail.com
- icon: linkedin
  icon_pack: fab
  link: https://www.linkedin.com/in/qzheng7/

# Important: use this to enable a list of pictures for all keynote pictures on the keynote speaker page.
user_groups:
- Keynote Speaker
---
**C2: LANL-Seagate's Early Prototype for Near-Data, SQL-Like Query Processing**

**Abstract:** High-performance computing data centers supporting large-scale simulation applications can routinely generate a tremendous amount of data. For cost-effective high bandwidth, many data centers have used tiered storage with warmer tiers made of flashes and cooler tiers provisioned with high-density rotational disk drives. While recent advances in storage media, high-speed interconnects, and systems software have greatly improved modern platforms’ ability to handle massive data, highly selective data retrievals, such as those in the form of SQL-like queries with predicates on potentially multiple data columns, tend to still experience excessive delays when unordered, unindexed data written in log-structured formats for high write bandwidth is subsequently read for interactive data analytics. Queries run slowly because an entire dataset may have to be transferred from storage to worker nodes, even when only a small portion is actually relevant. In the worst case, significant delays are experienced even when data is read from warm storage. A user sees even higher delays when data must be streamed from cool storage tiers.

In this presentation, we present C2, a research collaboration between Seagate and Los Alamos National Lab (LANL) for the lab's next-generation campaign storage. Campaign is a scalable cool storage tier at LANL managed by MarFS that currently provides 100 PBs of storage space for long-term data storage. Cost-effective data protection is done through multi-level erasure coding at both node level and rack level. To prevent users from potentially having to read back an entire dataset, C2 enables direct SQL-like query processing at the storage level by leveraging Seagate Kinetic Computational Storage Drives for near data processing. Combining computational storage technologies with erasure coding based data protection schemes for rapid data analytics over cool storage presents unique challenges in which individual disk drives may not be able to see complete data records and may not deliver performance required by high-level data applications. We discuss those challenges in the talk, share our designs, and report early results. Our results show that computational storage shows higher performance when host-storage interconnection bandwidth is a bottleneck, when host CPU is a bottleneck, and, perhaps surprisingly, when hosts do not have any obvious bottlenecks.

**Bio:** Qing Zheng is a Scientist in Los Alamos National Lab’s High-Performance Computing Division and a member of the Lab’s Ultrascale System Research Center. Qing performs I/O and storage research that guides the Lab’s future computing platform and storage infrastructure designs. Qing received his PhD in Computer Science from Carnegie Mellon University in 2021. Qing is known for his expertise in distributed filesystem metadata and large-scale data analytics. Qing’s work has been exhibited at local science museums, reported by national media, and recognized with multiple R&D 100 and Supercomputing Best Paper Awards.