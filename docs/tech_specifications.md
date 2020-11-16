# Technical specifications 

The protoSRC computing facility at the IAA-CSIC is an OpenStack cloud platform.   

The OpenStack cloud gathers 200 CPUs cores and 2.5 TB of memory across five compute hypervisors, plus 600+ TB of usable storage capacity managed by Ceph. The servers are interconnected in a 100Gbps network and the cluster is connected to RedIRIS (the Spanish National Research Network ) with a 10Gbps link.

 
## Virtual machine flavours 
The protoSRC provides seven ad-hoc flavors for virtual machines. Users can request the one more suitable for them.   

![](images/VM_flavours.png)

The SDC2 participants can choose between the following two flavours: 

spsrc.c8m32
8 vCPU cores
32 GB RAM
50 GB disk

spsrc.c16m64
16 vCPU cores
64 GB RAM
50 GB disk

## Software installed

The protoSRC provides the following base images for virtual machines from which users can request the most suitable for them:

- Ubuntu 18.04
- Ubuntu 20.04
- CentOS 8
- CentOS 7

Users with sudo access will be able to install their own software. 


