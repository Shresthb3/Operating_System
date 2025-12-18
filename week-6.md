# Phase 6: Performance Evaluation and Analysis

This stage will be devoted to testing the performance of the Linux server under various workload conditions to comprehend the operating system behaviour, detect the bottlenecks, and evaluate the effects of optimisation methods.

## Performance Testing Methodology

The testing methodology was structured as follows. Initial measurement values at **baseline** with little system load were taken to provide reference values. Tests that were workload-specific were then run on **CPU-intensive**, **memory-intensive**, **disk I/O intensive**, **network-intensive**, and **server-based applications**. Performance measurements were made periodically with in-built Linux monitoring applications and custom monitoring scripts [13].

## Resource Monitoring and Measurement

The following tools were used for resource monitoring and measurement:

| Resource | Monitoring Tools | Purpose |
| :--- | :--- | :--- |
| **CPU** | `top`, `mpstat` | To check CPU utilization. |
| **Memory** | `free`, `vmstat` | To record memory consumption. |
| **Disk I/O** | `iostat`, `fio` | To analyze disk I/O performance. |
| **Network** | `iperf3`, `ping` | To test network throughput and latency. |
| **Server Application** | Simulated client requests | To calculate service response time for the Apache web server. |

> **Figure 18: High CPU Usage**
>
> **Figure 19: High RAM utilisation**

## Load Testing and Bottleneck Identification

Load testing indicated that there were foreseeable resource usage issues as far as each type of application is concerned. Jobs that utilized high CPU rates led to prolonged processor utilization, whereas tests that were memory-intensive brought out limits on RAM allocation. Write/read throughput limits were revealed in disk I/O testing, and throughput limits were seen in network testing at large volumes of traffic. Such observations helped to obtain the **performance bottlenecks** within the system aspects.

## Modifications to Optimisation Performance

To enhance system performance, two main optimisation measures were used:

1.  **Background Service Reduction**: Background services that were not important were turned off in order to decrease the memory and CPU overhead.
2.  **Kernel and Application Tuning**: Parameters of kernel and application-level tuning, including the system scheduling and file system caching, were modified.

Post-optimisation testing indicated that measurable improvements had been made, including with respect to reduced CPU load, better memory availability, and better response times to server applications. These findings are supported by quantitative data obtained before and after optimisation.

## Visualisation of Performance and Analysis

The performance data was sorted into structured tables and plotted with the help of charts and graphs to demonstrate the trend of resource utilisation with time. These visual representations allowed the comparison of baseline, load, and optimised states clearly and allowed the drawing of evidence-related conclusions about the behaviour of the system and its efficiency.

## References

[13]: Placeholder for Citation 13

