# Phase 3: Application Selection for Performance Testing

## Selection of Applications and Workload Types

The applications were pooled according to resource intensity to provide a systematic test of critical performance dimensions of the server.

| Workload Type | Application | Purpose |
| :--- | :--- | :--- |
| **CPU-Intensive** | `stress-ng` | To put in place large stressed capacities. |
| **Memory-based** | `memtester` | To test memory consumption. |
| **Network-Intensive** | `iperf3` | As a measure of network throughput. |
| **Server Application** | `Apache2` | To test the service performance on client requests. |

This choice would provide a test of critical performance dimensions of the server in a systematic manner.

## Application Selection Matrix

*(Note: The content for the Application Selection Matrix was not provided in the source text. This section is included for structural completeness.)*

## Installation Documentation

All the chosen performance testing applications were installed on the Ubuntu Server via SSH. The installation of packages followed the **APT package manager**, and repositories have been updated, which provides a secure and reproducible deployment of all the necessary tools that are command-line-based.

> **Figure 4: Applications for performance testing installed**

![img alt](assets/images-2/Picture4.png)

## Monitoring Strategy

System commands (`top`, `vmstat`, `iostat`, `netstat`) and SSH custom scripts will yield performance measurements as data on CPU, memory, disk, and network utilisation, as time goes by. This system of planning enables quality performance assessment that is also quantitative.

## Expected Resource Profiles

The predictable resource utilisation patterns should be produced with each application, which allows monitoring the performance and revealing the bottlenecks.


