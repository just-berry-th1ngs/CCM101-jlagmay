# Cloud Storage Research

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Splits data into fixed-size blocks, each with a unique address. The OS/application manages how blocks are organized into files. Behaves like a raw hard drive attached to a server. | Databases, virtual machine disks, and applications needing low-latency, high-performance read/write access. | AWS EBS (Elastic Block Store) |
| **File Storage** | Organizes data in a hierarchical folder/file structure, accessed over a network using protocols like NFS or SMB. Multiple systems can read/write shared files. | Shared file systems for teams, content repositories, and applications needing simultaneous multi-user access. | AWS EFS (Elastic File System) |
| **Object Storage** | Stores data as discrete "objects" (data + metadata + unique ID) in a flat namespace called a bucket, accessed via HTTP APIs (e.g., S3 API). No folder hierarchy — just keys and metadata. | Storing massive amounts of unstructured data: images, videos, backups, static website assets. | AWS S3 (Simple Storage Service) |

## Why Object Storage is Best for User-Uploaded Images

Object storage is the best choice for the client's photo-sharing app because it can scale virtually infinitely without worrying about file system limits, unlike block or file storage. Each image is stored as an independent object with rich metadata, making it easy to retrieve, tag, and serve directly over HTTP/HTTPS to end users. It's also more cost-effective and durable for storing millions of large, rarely-modified files like photos.
