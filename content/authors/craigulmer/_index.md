---
# Display name
title: Craig Ulmer	

# Username (this should match the folder name)
authors:
- craigulmer

# Is this the primary user of the site?
superuser: false

# Role/position
role: Principal Member of Technical Staff

# Organizations/Affiliations
organizations: 
- name: Computation & Analysis for National Security Center
- name: Sandia National Laboratories
  url: https://www.sandia.gov/

# Short bio (displayed in user profile at end of posts)
bio: Craig Ulmer is a Principal Member of Technical Staff in the Computation & Analysis for National Security Center at Sandia National Laboratories in Livermore, California. His research focuses on adapting new hardware and software technologies to solve data-intensive problems more efficiently. During his 20 years of service at Sandia, he has worked with the scientific computing, nonproliferation, and cybersecurity mission spaces and led efforts to integrate SmartNICs, GPUs, NVMe, and FPGAs into production workflows. 

# Social/Academic Networking
# For available icons, see: https://sourcethemes.com/academic/docs/widgets/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.
social:
- icon: envelope
  icon_pack: fas
  link: mailto:cdulmer@sandia.gov
- icon: home
  icon_pack: fas
  link: https://craigulmer.com
- icon: linkedin
  icon_pack: fab
  link: https://www.linkedin.com/in/cdulmer/
- icon: github
  icon_pack: fab
  link: https://github.com/craigulmer

# Important: use this to enable a list of pictures for all keynote pictures on the keynote speaker page.
user_groups:
- Keynote Speaker
---
**Extending Composable Data Services into SmartNICs**

**Abstract:** Advanced, scientific-computing workflows rely on composable data service libraries to migrate data between different simulation and analysis jobs that run in parallel on a high-performance computing (HPC) platform. While these services are essential for staging and transforming in-transit data, they consume compute node resources that could otherwise be used for scientific work. Recent programmable network interface cards (or SmartNICs) provide a new alternative for hosting services that enables data management tasks to run in an isolated space at the compute node that does not impact host resources. In this talk we explore extending composable data services into SmartNICs and describe a software stack for services that uses Faodel and Apache Arrow. To illustrate how this stack operates, we present a case study that implements a distributed, particle-sifting service for reorganizing simulation results. Performance experiments from a 100-node cluster equipped with 100Gb/s BlueField-2 SmartNICs indicate that current SmartNICs can perform useful data management tasks, albeit at a lower throughput than hosts.

**Bio:** Craig Ulmer is a Principal Member of Technical Staff in the Computation & Analysis for National Security Center at Sandia National Laboratories in Livermore, California. His research focuses on adapting new hardware and software technologies to solve data-intensive problems more efficiently. During his 20 years of service at Sandia, he has worked with the scientific computing, nonproliferation, and cybersecurity mission spaces and led efforts to integrate SmartNICs, GPUs, NVMe, and FPGAs into production workflows. Prior to joining Sandia, Craig received a Ph.D. in Electrical and Computer Engineering from the Georgia Institute of Technology for his work in low-level communication software for resource-rich cluster computers.