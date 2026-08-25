# Client Recommendations

## Client A – Startup Company
**Recommended Platform: AWS**

AWS is well suited for a startup with a limited budget expecting rapid growth, since its Free Tier and pay-as-you-go pricing keep initial costs low while its auto-scaling infrastructure can grow with the business. Its large ecosystem of managed services also reduces the operational overhead of a small team. Startups commonly use AWS specifically because of the AWS Activate program, which offers credits for early-stage companies.
**Services:** Amazon EC2 (compute), Amazon S3 (storage for app assets), Amazon RDS (managed database for the mobile app backend).

## Client B – University
**Recommended Platform: Microsoft Azure**

Since the university already runs Windows Server, Microsoft 365, and Active Directory, Azure is the natural migration path because it integrates directly with those existing systems through Microsoft Entra ID. This minimizes retraining for IT staff and allows a smooth hybrid cloud transition rather than a full rebuild. Azure also offers education-specific licensing and pricing.
**Services:** Microsoft Entra ID (extending existing Active Directory), Azure Virtual Machines (hosting migrated Windows Server workloads), Azure Files (shared storage compatible with existing file servers).

## Client C – AI Research Company
**Recommended Platform: Google Cloud Platform**

GCP is the strongest fit for AI/ML research requiring high-performance computing, since it offers Vertex AI, TPUs (Tensor Processing Units), and GPU-backed compute purpose-built for machine learning workloads. Google's own research heritage in AI (e.g., TensorFlow) also means its tooling is closely aligned with cutting-edge ML frameworks. BigQuery further supports the large-scale data processing this kind of research needs.
**Services:** Vertex AI (model training and deployment), Compute Engine with GPUs/TPUs (high-performance compute), BigQuery (large-scale data analysis).

## Client D – Global E-Commerce Company
**Recommended Platform: AWS**

A global e-commerce platform needs highly available, auto-scaling infrastructure across many regions, which matches AWS's mature global infrastructure and its wide selection of scaling and reliability tools. AWS's CDN and DNS services help deliver low-latency shopping experiences worldwide, and its elastic load balancing handles unpredictable traffic spikes (e.g., sales events).
**Services:** Amazon EC2 Auto Scaling (handling traffic spikes), Amazon CloudFront (global content delivery), Elastic Load Balancing (distributing traffic across regions).

## Multi-Cloud Decision Matrix

| Business Requirement | Recommended Platform | Justification |
|---|---|---|
| Startup Company | AWS | Low-cost entry, startup credit programs, scalable as usage grows |
| Enterprise Organization | AWS or Azure | Mature governance tools and broad service catalog fit large, complex organizations |
| Microsoft Environment | Microsoft Azure | Native integration with Windows Server, AD, and Microsoft 365 |
| AI / Machine Learning | Google Cloud Platform | Vertex AI, TPUs, and strong data analytics tooling |
| Kubernetes Deployment | Google Cloud Platform | GKE is the most mature managed Kubernetes offering, built by Kubernetes' creator |
| Global Web Application | AWS | Largest global infrastructure footprint and mature auto-scaling/CDN tools |
