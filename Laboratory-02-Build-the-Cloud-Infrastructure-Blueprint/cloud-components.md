# Cloud Infrastructure Components

## Compute Resources
**Purpose:** Compute resources provide the processing power (CPU/RAM) that runs applications and services.
**Why it matters in cloud computing:** Compute is the core resource cloud providers sell (e.g. EC2, Azure VMs, GCE) - it determines how much workload a service can handle.
**In this KillerCoda environment:** [Reference your CPU model, core count, and RAM from infrastructure-report.md]

## Storage Resources
**Purpose:** Storage resources persist data - files, databases, logs - independently of running processes.
**Why it matters in cloud computing:** Cloud storage (e.g. S3, Azure Blob, GCS) must be durable, scalable, and separate from compute so data survives instance restarts or failures.
**In this KillerCoda environment:** [Reference your disk capacity and mounted file systems from infrastructure-report.md]

## Networking Resources
**Purpose:** Networking resources connect the server to other systems and to the internet, and control access via IP addressing and routing.
**Why it matters in cloud computing:** Networking (VPCs, subnets, security groups) determines how services communicate securely and how users reach them.
**In this KillerCoda environment:** [Reference your hostname and IP address from infrastructure-report.md]

## Operating System
**Purpose:** The OS manages hardware resources and provides the environment applications run in.
**Why it matters in cloud computing:** Cloud images are built on a specific OS/kernel version, which affects compatibility, security patching, and available tooling.
**In this KillerCoda environment:** [Reference your OS and kernel version from infrastructure-report.md]
