# Cloud Infrastructure Components

## 1. Compute Resources

Compute resources are the processing resources used to execute applications, services, and operating-system processes. The main compute resources include the CPU and memory allocated to a server.

### Example
The KillerCoda Linux server provides:

* **CPU:** Intel Xeon E312xx (Sandy Bridge, IBRS update)
* **CPU Cores:** 1
* **RAM:** 1.9 GiB

### Purpose

The CPU performs calculations and executes instructions, while RAM provides temporary working space for running processes and applications.

### Importance in Cloud Computing

Compute resources are fundamental to cloud computing because applications need processing power and memory to operate. Cloud providers allow organizations to provision and scale computing resources based on workload requirements.

### Relation to the KillerCoda Environment

The CPU and RAM provided by the KillerCoda Linux server represent the compute resources of the environment. These resources allow the Linux operating system and applications to run.

---

## 2. Storage Resources

Storage resources provide space for operating-system files, applications, configurations, and data.

### Example
The main storage filesystem identified on the KillerCoda server is:

* **Device:** `/dev/vda1`
* **Filesystem:** ext4
* **Capacity:** 19 GB
* **Mount Point:** `/`

Additional filesystems include `/dev/vda16` mounted at `/boot` and `/dev/vda15` mounted at `/boot/efi`.

### Purpose

Storage allows the server to retain files and information needed by the operating system and applications.

### Importance in Cloud Computing

Cloud storage provides scalable and accessible storage for applications and data. Cloud platforms offer different storage services for operating systems, application files, databases, backups, and user data.

### Relation to the KillerCoda Environment

The 19 GB `/dev/vda1` filesystem provides the primary storage space for the Linux environment. The `df -hT` command was used to investigate the server's storage capacity and mounted filesystems.

---

## 3. Networking Resources

Networking resources allow computers, servers, applications, and users to communicate with each other.

### Example
The main network configuration identified on the KillerCoda server is:

* **Network Interface:** `enp1s0`
* **IP Address:** `172.30.1.2/24`
* **Broadcast Address:** `172.30.1.255`

The server also has:

* `lo` — loopback interface
* `docker0` — Docker virtual network interface

### Purpose

Networking allows the server to communicate with other systems and services over a network.

### Importance in Cloud Computing

Cloud networking connects users, virtual machines, applications, databases, and other cloud resources. Network configuration also helps control how resources communicate with each other.

### Relation to the KillerCoda Environment

The `enp1s0` interface provides the primary network connection for the Linux server. Its IP address is `172.30.1.2/24`.

---

## 4. Operating System

An operating system manages computer resources and provides the environment required to run applications and services.

### Example
The KillerCoda server uses:

* **Operating System:** Ubuntu 24.04.4 LTS
* **Kernel:** 6.8.0-136-generic

### Purpose

The operating system manages CPU, memory, storage, networking, processes, users, and other system resources.

### Importance in Cloud Computing

Operating systems provide the software environment in which cloud applications and services run. Linux distributions are commonly used for cloud servers because they support a wide range of server applications, networking tools, automation technologies, and development environments.

### Relation to the KillerCoda Environment

Ubuntu 24.04.4 LTS provides the operating environment for the KillerCoda server. The Linux kernel manages the underlying system resources and allows applications to interact with the server.

---

## 5. Relationship Between the Components

The four infrastructure components work together to provide a functioning computing environment:

```text
Operating System
       |
       +---- manages ----> CPU / RAM
       |
       +---- manages ----> Storage
       |
       +---- manages ----> Network
       |
       +---- provides environment for ----> Applications
```

The CPU and RAM provide computing resources, storage provides persistent space for files and applications, networking enables communication, and the operating system manages these resources and provides the environment in which applications run.

## 6. Summary

The investigation demonstrated that a basic cloud infrastructure environment consists of multiple interconnected resources rather than a single component. The KillerCoda server provided compute resources through its CPU and RAM, storage through its virtual disk, networking through its network interfaces and IP address, and an operating system through Ubuntu Linux. Understanding these components provides a foundation for understanding larger cloud platforms such as AWS, Microsoft Azure, and Google Cloud.

