## Client A – Startup Company

**Recommended Platform: Amazon Web Services (AWS)**

AWS is recommended because the startup has a limited budget but expects rapid growth. AWS provides serverless services such as AWS Lambda, which allows the company to run application code without maintaining servers and pay based largely on usage. Amazon DynamoDB can provide a scalable database with on-demand capacity, while AWS Auto Scaling can automatically adjust resources as demand changes. These services allow the startup to begin with a small infrastructure footprint and scale as the mobile application gains users.

**Three services the client could use:**
1. AWS Lambda – serverless application backend
2. Amazon DynamoDB – scalable NoSQL database
3. Amazon S3 – storage for application files and media

---

## Client B – University

**Recommended Platform: Microsoft Azure**

Microsoft Azure is the best choice because the university already uses Windows Server, Microsoft 365, and Active Directory. Microsoft Entra ID (formerly Azure Active Directory) provides identity and access management and integrates with Microsoft 365 and on-premises environments. Azure also provides services for hosting Windows-based workloads and databases, making a gradual migration from existing infrastructure practical. Choosing Azure can reduce integration complexity because the university is already heavily invested in Microsoft's ecosystem.

**Three services the client could use:**
1. Microsoft Entra ID – identity and access management
2. Azure Virtual Machines – hosting Windows Server workloads
3. Azure SQL Database – managed relational database service

---

## Client C – AI Research Company

**Recommended Platform: Google Cloud Platform (GCP)**

GCP is recommended because the company develops Artificial Intelligence and Machine Learning applications that require high-performance computing. Google Cloud provides specialized AI and ML services, including Vertex AI, as well as GPU-enabled computing resources for demanding workloads. These services can support model training, experimentation, deployment, and inference. GCP is therefore a strong choice for a research company whose primary requirement is AI/ML performance and development capabilities.

**Three services the client could use:**
1. Vertex AI – machine learning development and deployment
2. Compute Engine – high-performance virtual machines and GPU workloads
3. Cloud Storage – scalable storage for datasets and trained models

---

## Client D – Global E-Commerce Company

**Recommended Platform: Google Cloud Platform (GCP)**

GCP is recommended because the company operates globally and requires highly available infrastructure with automatic scaling. Google Cloud Load Balancing can distribute traffic across healthy instances and route users toward appropriate infrastructure, while Compute Engine autoscaling can automatically add or remove resources as demand changes. Cloud Storage can provide scalable storage for product images, files, and other static content. This combination can help the e-commerce platform remain responsive during traffic spikes while avoiding unnecessary infrastructure costs during periods of lower demand.

**Three services the client could use:**
1. Google Cloud Load Balancing – distributes global application traffic
2. Compute Engine – scalable application infrastructure
3. Cloud Storage – scalable storage for products and media


# Cloud Platform Comparison


| Service Category | AWS | Azure | GCP |
|---|---|---|---|
| Virtual Machine | Amazon EC2 | Azure Virtual Machines | Google Compute Engine |
| Object Storage | Amazon S3 | Azure Blob Storage | Google Cloud Storage |
| Identity Management | AWS IAM | Microsoft Entra ID | Google Cloud IAM |
| SQL Database | Amazon RDS | Azure SQL Database | Cloud SQL |
| Kubernetes | Amazon EKS | Azure Kubernetes Service (AKS) | Google Kubernetes Engine (GKE) |

## Service Descriptions

### 1. Virtual Machine
- **AWS:** Amazon EC2
- **Azure:** Azure Virtual Machines
- **GCP:** Google Compute Engine

These services provide virtual machines that can run applications and operating systems in the cloud.

### 2. Object Storage
- **AWS:** Amazon S3
- **Azure:** Azure Blob Storage
- **GCP:** Google Cloud Storage

These services provide scalable storage for files, images, backups, videos, and other unstructured data.

### 3. Identity Management
- **AWS:** AWS IAM
- **Azure:** Microsoft Entra ID
- **GCP:** Google Cloud IAM

These services control authentication, identities, permissions, and access to cloud resources.

### 4. SQL Database
- **AWS:** Amazon RDS
- **Azure:** Azure SQL Database
- **GCP:** Cloud SQL

These services provide managed relational/SQL database capabilities without requiring the organization to manage all database infrastructure manually.

### 5. Kubernetes
- **AWS:** Amazon EKS
- **Azure:** Azure Kubernetes Service (AKS)
- **GCP:** Google Kubernetes Engine (GKE)

These services provide managed Kubernetes environments for deploying, managing, and scaling containerized applications.
