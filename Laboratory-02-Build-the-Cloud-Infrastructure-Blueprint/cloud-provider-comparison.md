# Cloud Provider Comparison

| Infrastructure Component | AWS | Microsoft Azure | Google Cloud Platform |
|---|---|---|---|
| Compute | EC2 | Virtual Machines | Compute Engine |
| Storage | S3 / EBS | Blob Storage / Managed Disks | Cloud Storage / Persistent Disk |
| Networking | VPC | Virtual Network (VNet) | VPC |
| Identity and Access Management (IAM) | AWS IAM | Microsoft Entra ID (Azure AD) | Cloud IAM |

## Guide Questions

**1. Which cloud provider offers the broadest range of services? Explain your answer.**

Amazon Web Services offers the broadest range of services among major cloud providers. This is because AWS launched years ahead of its competitors, giving it more time to build out its catalog — it now offers around 250 primary cloud services, surpassing both Azure and Google Cloud in niche capabilities. AWS also provides the widest array of specific instance types.

**2. Which cloud platform would you recommend for an organization that primarily uses Microsoft products? Why?**

Microsoft Azure is a no-brainer for Microsoft-focused companies and organizations. It works well with Windows Server, Office 365, and SQL Server, and it fits naturally with tools like Active Directory. Organizations can use a single login for both local computers and the cloud, so they don't need to build new tools just to make things fit together.

**3. Which platform is widely recognized for Artificial Intelligence (AI), Machine Learning (ML), and Kubernetes services?**

Based on my research, Google Cloud stands out here. Kubernetes itself is based on Google's internal system, Borg, and Google Cloud also developed TensorFlow and pioneered Tensor Processing Units (TPUs). TPUs are specialized hardware designed specifically to accelerate machine learning workloads, and Google Cloud has native support for running large-scale AI and ML training models inside containers.

**4. What similarities did you observe among the three cloud providers?**

All three providers offer high availability and provide virtual machines, serverless functions, object storage, block storage for disks, and managed relational databases. They also feature private cloud options and secure DNS management.
