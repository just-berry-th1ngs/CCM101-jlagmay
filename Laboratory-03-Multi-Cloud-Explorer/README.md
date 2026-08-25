# CCM101 Laboratory 3: Multi-Cloud Explorer

## Linux Investigation (Checkpoint 7)

Using a KillerCoda Ubuntu playground, the following system information was collected:

- **Operating System:** Ubuntu, Linux kernel 6.8.0-138-generic, x86_64 (GNU/Linux)
- **CPU Information:** 1 vCPU — Intel Xeon E312xx (Sandy Bridge), 2.0GHz, KVM virtualized
- **Memory:** 1.9 GiB total RAM, ~725 MiB free, 1.0 GiB swap
- **Disk Space:** 19 GB root filesystem (`/dev/vda1`), 13 GB available (30% used)

### If this Linux server were migrated to the cloud, which AWS, Azure, and GCP services could host it?

Given the modest specs (1 vCPU, ~2 GB RAM, ~20 GB disk), this server could be hosted on a small/burstable instance from any of the three providers:

- **AWS:** An **Amazon EC2** `t3.small` or `t3.micro` instance (Free Tier eligible), using **Amazon EBS** for the root disk. Both match the low CPU/RAM footprint seen here.
- **Azure:** An **Azure Virtual Machine** using the `B1s` or `B2s` Burstable series, which is designed for low, intermittent CPU usage — a good fit for this server's 1-vCPU workload.
- **GCP:** A **Compute Engine** `e2-small` instance, which offers a similarly small, cost-efficient VM size for lightweight Linux workloads.

All three options let the server be resized later (more vCPUs, RAM, or disk) if the workload grows, without needing to rebuild the server from scratch.

*(Insert screenshot: screenshots/killercoda-terminal.png)*
