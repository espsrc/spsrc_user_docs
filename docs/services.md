
# Services

## Virtual Machines

Virtual machines (VMs) in the protoSRC can be pre-configured with or without a desktop environment. All VMs can be accessed by SSH via public-key authentication (we will need your public key to give you access). We also offer a desktop environment that can be accessed using either an RDP client or via web-based access. You can access the desktop by installing an RDP client like Remmina in your computer (see [remote access](https://spsrc-user-docs.readthedocs.io/en/latest/access_guide/#remote-desktop) section). Alternatively, you can access the desktop environment from any browser using [Apache Guacamole](https://guacamole.apache.org).

A partially restricted **sudo** access will be granted to install new software and create new accounts for your collaborators.

Researchers will have access to a repository of ready-to-use [Singularity](https://sylabs.io) images. They can also request having [podman](https://podman.io) pre-configured to run containerised workloads.

Researchers will be able to select the resources of the VM, which can be adapted over time, and the Operating System they want to use. See what VM flavors and base images are available [here](tech_specifications.md).

VMs can have ad-hoc Block Storage for computing. We also offer Shared File System storage for long-term storage. 

Radioastronomers interested in using the [KERN](https://kernsuite.info) repository can request a VM with the latest Ubuntu 18.04 LTS pre-configured, or you can use the kern singularity images available in all machines.


## Scientific support 

We provide scientific support to the preparation of observational proposals with SKA precursor and pathfinder radiotelescopes. [Contact us](https://spsrc-user-docs.readthedocs.io/en/latest/about_us/#contact). 


## Reproducibility and Open Science advise

We help users to follow Open Science and Reproducibility [best practices](https://www.go-fair.org/fair-principles/). We offer a centralised catalogue of containerised images that can be found at ```/mnt/software/containers/ ```

![image](https://user-images.githubusercontent.com/22152978/140042206-1f6abb02-427c-474a-a9d1-cbe300de4987.png)


## Jupyter Notebooks service

We offer a [Jupyter](https://jupyter.org/hub) platform for data exploration, data analysis and workflows using a web interface. This service is available also for training activities, courses and schools. 


## Batch processing service with Slurm 

If you are interested in the batch processing service through slurm please contact us. 

## ContainersHub 

The protoSRC Container Registry provides a catalog of ready-to-use applications and services from a virtual machine instance, also providing the ability to include your own software in the repository. 



# Resource accounting information

The parameters used for accounting the resource usage of the protoSRC in each of the service categories offered are desccribed as follows. While no costs are currently charged for the use of these resources, this accounting allows for a better evaluation of the support provided in quantifiable terms, ensuring equitable distribution.

### A) Support Services

Billing unit: €/hour Cost: €34.70/hour

### B) Virtual Infrastructure Services

Virtual machine instances  
Billing unit: €/day

| Flavor                    | vCPU | RAM  | Storage (GB) | Cost (€/day) |
|-------------------------------|----------|----------|------------------|------------------|
| Flavor 1                       | 2        | 2 GB     | 50 GB            | €0.67            |
| Flavor 2                       | 4        | 8 GB     | 50 GB            | €2.02            |
| Flavor 3                       | 8        | 16 GB    | 50 GB            | €4.03            |
| Flavor 4                       | 8        | 32 GB    | 50 GB            | €6.72            |
| Flavor 5                       | 16       | 32 GB    | 50 GB            | €8.10            |
| Flavor 6                       | 24       | 32 GB    | 50 GB            | €9.41            |
| Flavor 7                       | 32       | 128 GB   | 50 GB            | €26.88           |

  
Mass storage
- Type: Block Storage  
  Billing unit: €/GB Cost: €0.018/GB
- Type: CephFS  
  Billing unit: €/GB Cost: €0.023/GB



### C) Analysis Platform Services
- Use of Batch Processing Service with Slurm  
Billing unit: €/hour Cost: €1.56/hour

- High availability JupyterHub  
Billing unit: €/user/month Cost per user: €15/month

- Container and software registry service (ContainersHub)  
Billing unit: €/service One-time cost: €10

