# Phase 7: Security Audit and System Evaluation

This audit gives a general analysis of system security positioning and confirms that best practices have been adhered to in the administration of Linux servers.

## Security Audit Methodology

Various auditing tools and techniques were used to have a comprehensive assessment. **Lynis** was used to perform a basic security scan to evaluate the host system hardening, configuration problems, and adherence to security standards. Security on the network level was assessed with the help of **Nmap** to detect all the open ports and the services available. More verification was carried out in access control validation, service inventory analysis, and configuration review of the system.

## Lynis Security Audit

The execution of Lynis on the server produced a comprehensive report on the security assessment. The initial scan showed room for improvement, such as service hardening and configuration suggestions. The conclusion was that after remediation measures, the **hardening index** was improved, according to a second scan by Lynis, which indicated that the taken security measures were effective.

> **Figure 20: Lynis Audit complete**

## Network Security Assessment with Nmap

**Nmap** was used to scan the server from the workstation to analyze the network exposure. The findings affirmed that only ports that were necessary, and especially SSH, were open and accessible. The firewall filtered all other ports or closed them, which confirmed the effectiveness of **UFW rules** and network segmentation.

> **Figure 21: Nmap Scan of the Server complete**

## Service Inventory and Justification

A complete inventory of running services was made to ensure only necessary services were operational. All operational services were checked and validated according to their functionality or protection of the system. Non-utilized or redundant services were switched off as much as possible so as to reduce the attack surface.

> **Figure 22: Services running on Ubuntu Server**

## Residual Risk Assessment

Although the security posture is strong, there are still complementary risks, such as the presence of **zero-day vulnerabilities** and possible misconfigurations. Such risks are mitigated by automatic updating, constant oversight, and periodic security audits. In general, the system proves to be secure enough and resistant to widespread threats.

# Conclusion and Reflection

This coursework has provided a detailed discussion on how Linux can be configured as a server, hardened, and performance assessed, all within a headless controlled environment. By applying the **dual-system architecture** and only executing the administration through the command-line (SSH), the real-world training skills required to administer a system were acquired and enhanced.

During the evaluation, a secure and optimised Linux server has been successfully installed, and it includes the best security practices in the industry, including key-based SSH authentication, firewall enforcement, mandatory access control, intrusion detection, and automatic patch management. The formal performance analysis showed what various workloads do with system behaviour and how monitoring, bottleneck analysis, and optimisation can enhance the resource utilisation and system sensitivity.

This security audit stage confirmed the quality of adopted controls and the importance of a periodic system test through the deployment of the host-based and network-based tools. The security check and surveillance through the use of scripts illustrated further the advantage of **automation** in system integrity and operational consciousness.

When looking back on this learning experience, the evaluation provided was helpful in forming the theoretical knowledge and putting it into practice. The problems encountered in the process of set-up and testing created skills of problem-solving and critical thinking. In general, the project has not only enhanced understanding of the basic requirements of Linux administration but has also given one a clear insight into how to design, secure, and optimise the server operating systems in the professional computing environment.

