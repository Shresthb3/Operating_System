# Phase 2: Security Planning and Testing Methodology

## Security Baseline Design

A detailed **security baseline** determines the lowest security requirements of the server and provides uniformity and robustness to the server with regard to attacks. The **SSH hardening**, **firewall definition**, access control, automated security updates, and management of user privileges are some of the key elements of the baseline. This baseline can be used to check the level of compliance and also at which the level of extra security measures put in the further stages is checked [5].

## Performance Testing Plan

The method of performance testing is a process that entails observing the CPU, memory, disk I/O, and network performance under varying workloads. Remote monitoring is done through SSH and with scripts that gather metrics of the system every so often. Measurements of the unmodified system are measured as **baseline measurements**, and after measuring the measurements, the workload-based testing is applied to the CPU-intensive, memory-intensive, I/O intensive, network-intensive, and server applications. The testing plan records the steps, anticipated results, and performance guidelines so that they can be collected in a structured manner and analyzed quantitatively [6].

## Checklist of Security Configurations

A specific checklist will make sure that each security configuration will be uniformly applied and provable. Key items include:

*   Implementation of SSH authentication with the use of key-based authentication and the disabling of root login.
*   Setting of the **UFW firewall** to allow only the designated workstation.
*   Introducing compulsory access control with **AppArmor**.
*   Allowing automatic security updates in order to update vulnerabilities.
*   User privilege control and administrative access control.

## Threat Model and Mitigation Strategies

The following table summarizes the identified threats and their corresponding mitigation strategies:

| Threat | Mitigation Strategy | Citation |
| :--- | :--- | :--- |
| SSH Unauthorized Access | Reduced by firewall and key-based authentication. | |
| Brute-Force Attacks | Reduced with the help of **fail2ban** and tracking of failed attempts to log into the system. | [7] |
| Privilege Escalation | Mitigated with the help of **AppArmor**, least privilege policies, and the segregation of administrative users. | [8] |

> **Figure 3: Tools needed installed**
> 
> ![img alt](assets/images-2/Picture3.png)

This step provides a structured base for ensuring that the server is secured and monitored in a structured environment and that the further configuration and testing phases are implemented on a reliable and well-documented base.
