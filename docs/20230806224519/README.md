# 20230806224519
# Docker's Foundation

Containers are just a process/a group of processes running in isolation with
the help of Linux namespaces and control groups which both are a commodity of
Linux kernel.

Use of the union file system is one of the strong 'design' suits of Docker.
Each line in a dockerfile is basically a layer. They consists a series of
read-only layers stacked on each other. Each layer contains only the difference
that other layers do not have. Layers share common data, returning a great
performance and good utilization of computing resources.

Apart from read-only layers, there is a writable layer at up top. Any changes
made to a container are isolated from other layers and kept in writable/container
layer, so multiple containers can share the same base and read-only layers while
containers are being unique without having duplicate files.

#docker #ufs #cow

