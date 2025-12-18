# Phase 4: Initial System Configuration & Security Implementation

This stage is aimed at implementing the Linux server and establishing the basic security controls to provide safe remote administration. Each of the configurations was remotely achieved through **SSH** by the workstation system and adhered to the administrative limitations set in the assessment.

## SSH Key-based Authentication Implementation

The SSH service had been set to utilize **key-based authentication**, and password login was disabled. The workstation was used to generate an SSH key pair, and the public key was copied safely to the server's authorized keys file. **Root login** and **password authentication** were also turned off to decrease the attack surface and reduce unauthorized access [9].

> **Figure 5: SSH key generated and added on Server**
>
> **Figure 6: Disabling Root Login and Password authentication**
>
> **Figure 7: SSH key added to authorised keys**

## Firewall Ruleset and Firewall Configuration

The **Uncomplicated Firewall (UFW)** was configured on the server to regulate the incoming and outgoing traffic. The firewall was set to allow the IP address of the workstation to have SSH access, but not to allow access by a remote host, effectively isolating access to a trusted network. All other inbound connections were rejected by default, providing a network-level **least privilege principle** [10].

> **Figure 8: SSH restarted and UFW enabled**

## User and Privilege Management

An administrative user who was not a root was created to do the routine management activities. This user was given **sudo privileges**, but direct root access was revoked. Such a division of responsibilities minimizes the chances of unintentional damage in the system and scales the effects of misused credentials [11].

## Remote Administration Evidence

The workstation was able to establish a successful SSH connection with the Ubuntu Server, which is an indicator that key-based authentication and firewall restrictions could be implemented as programmed features. The command line was used to perform all system administration functions such as user management, firewall setup, and service restart.

> **Figure 9: Connection to Ubuntu Server successful**

## Configuration File Comparison

Prior-and-comparisons between key configuration files, including `/etc/ssh/sshd.config` and UFW rulesets, were also reported in an attempt to create clear evidence of changes executed in this stage. Such comparisons help to provide transparency, reproducibility, and auditability of system configurations.

This stage provides a safe base for the upper security control measures and performance monitoring adopted in the later stages.

## References

[9]: Placeholder for Citation 9
[10]: Placeholder for Citation 10
[11]: Placeholder for Citation 11

