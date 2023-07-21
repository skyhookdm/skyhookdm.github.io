---
# Display name
title: Jayjeet Chakraborty

# Username (this should match the folder name)
authors:
- jayjeet.chakraborty

# Is this the primary user of the site?
superuser: false

# Role/position
role: PhD Student

# Organizations/Affiliations
organizations: 

# Short bio (displayed in user profile at end of posts)
bio: Jayjeet Chakraborty is a PhD student at the University of California, Santa Cruz. He is advised by Carlos Maltzahn. His research interests include Data management and Database systems, Computational storage systems, Distributed systems, and Systems in general. For his PhD, he is working with Argonne National Labs on building a hardware-accelerated columnar data transport frameworks leveraging RDMA.

# Social/Academic Networking
# For available icons, see: https://sourcethemes.com/academic/docs/widgets/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.
social:
- icon: envelope
  icon_pack: fas
  link: mailto:jayjeetc@ucsc.edu
- icon: linkedin
  icon_pack: fab
  link: https://www.linkedin.com/in/jayjeetc

# Important: use this to enable a list of pictures for all keynote pictures on the keynote speaker page.
user_groups:
- Keynote Speaker
---
**Fast Columnar Data Transport using RDMA**

**Abstract:** The amount of data stored in data centers worldwide is increasing faster than ever. Much of this data is stored to process, analyze, and extract valuable insights. Primarily, large datasets are stored in dumb storage servers inside data centers. To perform analysis and compute on this data, it must first be transported to compute servers, usually with big DRAMs and huge processing capabilities, where the data is processed and result sets sent to the client. Traditional data transport frameworks use TCP/IP as their underlying protocol and therefore require the users to provide with a single contiguous buffer for transfer to the framework. We observe that this approach adds a severe overhead when transferring batches of columnar records. Columnar tables consist of several buffers scattered in the memory, each representing a particular column and its metadata. Serializing these buffers into a single buffer requires doing multiple memory copies. To avoid this serialization overhead while transfer columnar batches over the wire, we propose using RDMA as a potential solution to this problem. In this paper, we explore transporting columnar result sets over RDMA from a server to a client and compare this approach with a state-of-the-art TCP/IP based transport framework. We show that using RDMA for columnar data transport provides up to 2x higher throughput. 

**Bio:** Jayjeet Chakraborty is a PhD student at the University of California, Santa Cruz. He is advised by Carlos Maltzahn. His research interests include Data management and Database systems, Computational storage systems, Distributed systems, and Systems in general. For his PhD, he is working with Argonne National Labs on building a hardware-accelerated columnar data transport frameworks leveraging RDMA.

**Contact:** Jayjeet Chakraborty; e-mail: jayjeetc@ucsc.edu
