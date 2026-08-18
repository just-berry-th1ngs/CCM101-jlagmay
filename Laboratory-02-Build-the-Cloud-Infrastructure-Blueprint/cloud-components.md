# Cloud Infrastructure Components

## Compute Resources
**Purpose:** Compute resources provide the processing power (CPU/RAM) that runs applications and services.
**Why it matters in cloud computing:** Compute is the core resource cloud providers sell (e.g. EC2, Azure VMs, GCE) - it determines how much workload a service can handle.
**In this KillerCoda environment:** My server is running on an Intel Xeon E312xx (Sandy Bridge) CPU at 2.0GHz with only 1 core, and 1.9Gi total RAM (859Mi free, 1.5Gi available). It's a small setup, which shows how even a lightweight simulated instance still counts as a real compute resource - it just has less capacity than a production server would.

## Storage Resources
**Purpose:** Storage resources persist data - files, databases, logs - independently of running processes.
**Why it matters in cloud computing:** Cloud storage (e.g. S3, Azure Blob, GCS) must be durable, scalable, and separate from compute so data survives instance restarts or failures.
**In this KillerCoda environment:** My main filesystem `/dev/vda1` is ext4, 19G total with 5.4G used (30% usage), mounted on `/`. There's also `/dev/vda16` (703M, mounted on `/boot`) and `/dev/vda15` (vfat, 105M, mounted on `/boot/efi`). Having separate mounts like this shows how storage is organized by purpose - one for the system, one for boot files.

## Networking Resources
**Purpose:** Networking resources connect the server to other systems and to the internet, and control access via IP addressing and routing.
**Why it matters in cloud computing:** Networking (VPCs, subnets, security groups) determines how services communicate securely and how users reach them.
**In this KillerCoda environment:** My server's hostname is `ubuntu`, with IP addresses `172.30.1.2` and `172.17.0.1`. These are what let this instance actually be reached and communicate with other machines - without them, it would just be an isolated box with no way in or out.

## Operating System
**Purpose:** The OS manages hardware resources and provides the environment applications run in.
**Why it matters in cloud computing:** Cloud images are built on a specific OS/kernel version, which affects compatibility, security patching, and available tooling.
**In this KillerCoda environment:** My server is running Ubuntu 24.04.4 LTS (Noble Numbat) on kernel 6.8.0-136-generic. Knowing the exact OS and kernel version matters because it tells me what commands, packages, and security patches are actually compatible with this machine.
