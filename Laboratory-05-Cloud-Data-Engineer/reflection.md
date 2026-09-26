# Reflection

This laboratory activity helped me understand why different types of cloud storage are designed for different purposes. Object storage is more suitable for millions of user-uploaded photos because photos are unstructured data and can be stored as individual objects. Object storage can also scale to handle a very large number of files while allowing applications to access them through APIs. Block storage is more appropriate for applications that require a disk-like storage system with frequent low-level read and write operations.

Docker made deploying MinIO easier because I did not need to manually install and configure all of its dependencies on the Linux environment. Instead, I was able to run MinIO inside a container using a Docker command. Docker also allowed me to configure ports, environment variables, and persistent storage in the same deployment process. This made the deployment more consistent and easier to manage.

A bucket is a logical container used to organize and store objects in an object storage system. In this activity, I created a bucket called `client-photos` and uploaded a test file to demonstrate how object storage works.

Enterprises can reduce the risk of data loss when a physical server crashes by using redundancy, backups, replication, and distributed storage. Data can be stored across multiple servers or locations so that a failure of one physical machine does not automatically result in permanent data loss. Regular backups and recovery procedures are also important for protecting business data.

My confidence with Linux command-line tools is also improving through this activity. I used commands to pull Docker images, create volumes, run containers, check container status, and troubleshoot deployment problems. Working through the MinIO deployment errors helped me become more comfortable reading terminal output and finding practical solutions instead of relying only on graphical interfaces.

