# Technical specifications 

The protoSRC computing facility at the IAA-CSIC runs an OpenStack cloud with an aggregate of 200 CPUs cores
and 2.5 TB of memory distributed across five compute hypervisors, plus 600 TB of usable storage managed by Ceph.
OpenStack and Ceph are interconnected internally with a 100Gbps network and the cluster is connected to
[RedIRIS](https://www.rediris.es/) (the Spanish National Research Network ) with a 10Gbps link.

## Virtual machine flavors 

The protoSRC provides the following default flavors but talk to us if you need something specific:

| Flavor Name | vCPUs | RAM   | Root Disk |
|:-----------:|:-----:|:-----:|:---------:|
| spsrc.c2m4  | 2     | 4 GB  | 50 GB |
| spsrc.c4m8  | 4     | 8 GB  | 50 GB |
| spsrc.c8m32 | 8     | 32 GB | 50 GB |

## Virtual machine images

We currently support the following base images for virtual machines:

- Ubuntu 18.04
- Ubuntu 20.04
- CentOS 8
- CentOS 7

