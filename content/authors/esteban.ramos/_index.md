---
# Display name
title: Esteban Ramos

# Username (this should match the folder name)
authors:
- esteban.ramos

# Is this the primary user of the site?
superuser: false

# Role/position
role: PhD Student

# Organizations/Affiliations
organizations: 
- name: University of California, Santa Cruz
  url: https://www.ucsc.edu/

# Short bio (displayed in user profile at end of posts)
bio: Esteban Ramos is a PhD student at the University of California, Santa Cruz. He is advised by Dr. Peter Alvaro. He is interested in distributed systems, data management systems, and networking. He is currently working on projects that seek to minimize overhead introduced by RPCs in microservice applications.  


# Social/Academic Networking
# For available icons, see: https://sourcethemes.com/academic/docs/widgets/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.
social:
- icon: envelope
  icon_pack: fas
  link: mailto:esiramos@ucsc.edu
- icon: linkedin
  icon_pack: fab
  link: https://www.linkedin.com/in/esteban-ramos-956a34174/

# Important: use this to enable a list of pictures for all keynote pictures on the keynote speaker page.
user_groups:
- Keynote Speaker
---
**Split gRPC: An Isolation Architecture for RPC Stacks on SmartNICs**

**Abstract:** Remote procedure calls are a major contributor to performance variance in distributed systems due to lack of isolation and contention on shared resources. In this talk, I will introduce the novel architecture we build to address this problem, and cover our experience in implementing a prototyp e on the popular RPC framework, gRPC. The basic idea is to partition RPC applications into two communicating components: one dedicated to user-implemented business logic, and one dedicated to RPC infrastructure processing. The infrastructure process can be run on a dedicated core or on a smart NIC (e.g., IPU or DPU), providing effective physical isolation and predictable performance. An evaluation of a proof-of-concept prototype shows that the split architecture adds modest overhead for average case latency, but allows for lower latency and and higher throughput under host CPU load.


**Bio:** Esteban Ramos is a PhD student at the University of California, Santa Cruz. He is advised by Dr. Peter Alvaro. He is interested in distributed systems, data management systems, and networking. He is currently working on projects that seek to minimize overhead introduced by RPCs in microservice applications.  

**Contact:** Esteban Ramos; e-mail: esiramos@ucsc.edu
