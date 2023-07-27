---
# Display name
title: Matthew Curry	

# Username (this should match the folder name)
authors:
- matthew.curry

# Is this the primary user of the site?
superuser: false

# Role/position
role: Principal Member of Technical Staff

# Organizations/Affiliations
organizations: 
- name: Center for Computing Research (CCR)
  url: https://www.sandia.gov/ccr/
- name: Sandia National Laboratories
  url: https://www.sandia.gov/

# Short bio (displayed in user profile at end of posts)
bio: Matthew Curry has a wide variety of research interests, mostly pertaining directly to data storage in supercomputing environments, including parallel and distributed storage systems, erasure coding and fault tolerance, low-level (block or object) storage devices, and heterogeneous computing (e.g., GPUs, accelerators). He graduated with a Ph.D. in Computer Science at University of Alabama at Birmingham under the advisement of Dr. Anthony Skjellum.

# Social/Academic Networking
# For available icons, see: https://sourcethemes.com/academic/docs/widgets/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.
social:
- icon: envelope
  icon_pack: fas
  link: mailto:mlcurry@sandia.gov
- icon: linkedin
  icon_pack: fab
  link: https://www.linkedin.com/in/curryml/
- icon: github
  icon_pack: fab
  link: https://github.com/matthewcurry

# Important: use this to enable a list of pictures for all keynote pictures on the keynote speaker page.
user_groups:
- Keynote Speaker
---
**An HPC-Oriented Runtime Environment for Enabling Computational Storage**

**Abstract:** There are at least two methods for enabling computational storage workflows on embedded storage hardware. The first revolutionary path is to port applications to relatively lightweight storage abstractions that allow simple software stacks. A second evolutionary path is to enable existing storage abstractions by porting existing libraries and utilities to computational storage hardware. While the evolutionary path is a good stop-gap measure until applications can be prepared, porting significant dependency chains for complex libraries to the required interesting architectures can be a significant hurdle.  
 
In this talk, I will describe the Advanced Tri-lab Software Environment (ATSE). ATSE is a traditional HPC software stack for testbed systems. As a full-featured stack, it is able to provide complex I/O libraries such as HDF5, NetCDF, CGNS, Exodus, and others. Crucially, ATSE has been demonstrated to port to many variants of Arm and RISC-V processors, allowing use on low-power hardware often found in computational storage devices. Along with the stack itself, this talk will touch on techniques and facilities allowing ATSE’s high levels of portability.

**Bio:** Matthew Curry has a wide variety of research interests, mostly pertaining directly to data storage in supercomputing environments, including parallel and distributed storage systems, erasure coding and fault tolerance, low-level (block or object) storage devices, and heterogeneous computing (e.g., GPUs, accelerators). He graduated with a Ph.D. in Computer Science at University of Alabama at Birmingham under the advisement of Dr. Anthony Skjellum.