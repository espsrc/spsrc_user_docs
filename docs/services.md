
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

