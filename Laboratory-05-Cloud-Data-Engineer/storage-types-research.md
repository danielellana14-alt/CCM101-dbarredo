# Storage Types Research

Cloud storage can be categorized into three primary types: Block Storage, File Storage, and Object Storage. Each type is designed for different workloads and provides different methods of storing and accessing data.

## Comparison of Cloud Storage Types

| Storage Type       | Description                                                                                                                                                       | Primary Use Case                                                                                      | Cloud Provider Example                 |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | -------------------------------------- |
| **Block Storage**  | Stores data in fixed-size blocks that can be independently accessed and managed. It behaves similarly to a traditional hard drive or disk attached to a computer. | Best for operating systems, databases, and applications that require fast and consistent disk access. | **AWS Elastic Block Store (EBS)**      |
| **File Storage**   | Stores data as files organized into directories and folders. Multiple computers or applications can access the same file system over a network.                   | Best for shared files, content repositories, and applications that require a shared file system.      | **Amazon Elastic File System (EFS)**   |
| **Object Storage** | Stores data as objects along with metadata and a unique identifier. Objects are stored in a flat structure called a bucket.                                       | Best for large amounts of unstructured data such as images, videos, documents, backups, and archives. | **Amazon Simple Storage Service (S3)** |

## Why Object Storage is Suitable for the Client

Object Storage is well suited for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as user-uploaded images. It can provide scalable storage while allowing applications to access objects through APIs, making it practical for applications that may need to store millions of photos.

