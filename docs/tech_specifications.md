# Technical specifications

The protoSRC computing facility at the IAA-CSIC runs an OpenStack cloud with the following resources:

**CPU and GPU cores:**

- Intel nodes: 240 cores
- AMD nodes: 384 cores
- GPU node: 96 cores

**RAM (total: ~8.3 TB):**

- Intel nodes: 9.6 GB RAM per core in 5 nodes and 25.6 GB RAM per core in 1 node
- AMD nodes: 12 GB RAM per core
- GPU node: 8 GB RAM per core

**Storage:**

- 1.47 PB of raw SSD storage
- 1.15 PB of raw HDD storage

**Network:**

OpenStack and Ceph are interconnected internally with a 100 Gbps network, and the cluster is connected to
[RedIRIS](https://www.rediris.es/) (the Spanish National Research Network) with a 10 Gbps link.


## Virtual machine flavors 

The protoSRC provides the following default flavors but talk to us if you need something specific:

| Flavor Name | vCPUs | RAM   | Root Disk |
|:-----------:|:-----:|:-----:|:---------:|
| spsrc.c2m4  | 2     | 4 GB  | 50 GB |
| spsrc.c4m8  | 4     | 8 GB  | 50 GB |
| spsrc.c8m32 | 8     | 32 GB | 50 GB |

## Virtual machine images

We currently support the following base images for virtual machines:

- Ubuntu 24.04
- Ubuntu 26.04
- CentOS

