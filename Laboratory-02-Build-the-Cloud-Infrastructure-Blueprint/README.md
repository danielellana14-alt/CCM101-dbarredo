# Laboratory 02 – Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory focused on investigating a Linux server environment and identifying the fundamental infrastructure components used in cloud computing. The activity included examining compute, memory, storage, networking, and operating system resources using Linux commands in a KillerCoda environment.

The laboratory also involved researching and comparing equivalent infrastructure services from Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP). Finally, a basic cloud infrastructure blueprint was created to demonstrate how users, networks, compute resources, and storage are connected.

## Objectives

* Investigate a Linux cloud server environment.
* Identify compute, memory, storage, networking, and operating system resources.
* Understand the purpose of fundamental cloud infrastructure components.
* Compare equivalent services offered by AWS, Microsoft Azure, and Google Cloud.
* Design a simple cloud infrastructure architecture.
* Document technical findings using Markdown.
* Organize and maintain laboratory work using GitHub.

## Environment Investigated

The laboratory used a Linux server provided through KillerCoda.

### Server Information

| Resource               | Result                                        |
| ---------------------- | --------------------------------------------- |
| Operating System       | Ubuntu 24.04.4 LTS                            |
| Kernel Version         | 6.8.0-136-generic                             |
| CPU Model              | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| CPU Cores              | 1                                             |
| Total RAM              | 1.9 GiB                                       |
| Main Disk              | 19 GB                                         |
| Hostname               | ubuntu                                        |
| Main Network Interface | enp1s0                                        |
| IP Address             | 172.30.1.2                                    |

## Infrastructure Components Investigated

The main cloud infrastructure components investigated were:

### Compute

The CPU and RAM provide the processing resources required to run applications and operating-system processes.

### Storage

The server's virtual disk provides persistent storage for the operating system, applications, configuration files, and other data.

### Networking

The server's network interface and IP address provide connectivity and allow communication with other systems and services.

### Operating System

Ubuntu Linux manages the server's hardware and software resources and provides the environment required to run applications.

## Linux Commands Used

The following commands were used to investigate the server:

```bash
cat /etc/os-release
uname -r
lscpu | grep "Model name"
nproc
free -h
df -hT
hostname
hostname -I
ip addr
```

These commands provided information about the operating system, kernel, CPU, memory, storage, hostname, and network configuration.

## Cloud Provider Research

The laboratory compared the following equivalent services:

| Infrastructure Component | AWS        | Microsoft Azure                 | Google Cloud     |
| ------------------------ | ---------- | ------------------------------- | ---------------- |
| Compute                  | Amazon EC2 | Azure Virtual Machines          | Compute Engine   |
| Storage                  | Amazon S3  | Azure Blob Storage              | Cloud Storage    |
| Networking               | Amazon VPC | Azure Virtual Network           | Google Cloud VPC |
| IAM                      | AWS IAM    | Microsoft Entra ID / Azure RBAC | Cloud IAM        |

## Cloud Architecture

A simple cloud infrastructure blueprint was created to demonstrate the relationship between the main infrastructure components.

The architecture follows this flow:

```text
User
  ↓
Internet
  ↓
Cloud Network / VPC
  ↓
Compute Resource / Linux VM
  ↓
Storage
```

The architecture diagram is available in:

```text
screenshots/cloud-architecture.png
```

## Tools Used

* KillerCoda
* Ubuntu Linux
* Linux Terminal
* GitHub
* Git
* Markdown
* diagrams.net

## Skills Learned

Through this laboratory, I practiced Linux server investigation, identification of cloud infrastructure resources, cloud provider comparison, basic cloud architecture design, Markdown documentation, and GitHub repository management.

## Challenges Encountered

One challenge was understanding how the different Linux resources relate to cloud infrastructure concepts. Another challenge was comparing AWS, Microsoft Azure, and Google Cloud because each provider uses different names for services that perform similar functions.

## Conclusion

This laboratory provided practical experience in identifying the basic components that make up a cloud infrastructure environment. Investigating the KillerCoda Linux server and comparing major cloud providers helped demonstrate how compute, storage, networking, operating systems, and access management work together to support cloud applications and services.

