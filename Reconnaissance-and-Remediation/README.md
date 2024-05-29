# Reconnaissance-and-Remediation

### Project Overview

In this project, I will demonstrate the comprehensive process of vulnerability management by taking on the roles of both an attacker and an administrator. The aim is to identify security vulnerabilities in a target machine and then perform remediation to secure it. The target in this scenario is a Windows 10 host machine, and I will be using a Kali Linux Virtual Machine to conduct the initial attack and subsequent vulnerability assessments.

#### Tools and Techniques:

1. **Nmap**:
   - **Purpose**: As a widely-used network scanning tool, Nmap will be utilized to perform an initial reconnaissance of the Windows 10 host machine. This includes discovering open ports, services running on these ports, and other network-level information.
   - **Usage**: By executing various Nmap scans, I will gather preliminary data that will help in identifying potential entry points and vulnerabilities.

2. **Nessus**:
   - **Purpose**: Nessus is a powerful vulnerability scanning tool that provides in-depth analysis of the target machine’s security posture. It can identify a wide range of vulnerabilities, from missing patches to misconfigurations.
   - **Usage**: Running Nessus on the Kali Linux VM, I will conduct comprehensive scans of the Windows 10 host machine. The scans will highlight specific vulnerabilities, including CVEs (Common Vulnerabilities and Exposures) and provide detailed reports on the severity and impact of each finding.

#### Target Acquisition and Scanning:

- **Nmap Scanning**:
  - Initial network scans will be performed using Nmap to map out the network and identify the Windows 10 host machine.
  - Detailed service and version detection scans will provide insights into the operating system, running services, and potential vulnerabilities.

- **Nessus Vulnerability Assessment**:
  - A full vulnerability assessment will be conducted using Nessus. This step involves running targeted scans that cover the entire host machine, examining various components and configurations to uncover security weaknesses.

#### Remediation Process:

1. **Action1**:
   - **Purpose**: Action1 is a cloud-based endpoint security management tool that facilitates the identification and remediation of vulnerabilities on the host machine.
   - **Usage**: Inside the Windows 10 host machine, Action1 will be deployed to perform a detailed vulnerability scan, corroborating the findings from Nessus. The tool will list all detected vulnerabilities and provide options for remediation.

2. **Applying Remediation**:
   - **Patching**: Using Action1, I will deploy necessary security patches to address the identified vulnerabilities. This includes updating software and applying fixes to known issues.
   - **Configuration Changes**: Adjustments to system settings and configurations will be made to enhance security, such as disabling unnecessary services or modifying access controls.

#### Verification and Rescanning:

- **Rescanning with Nessus and Nmap**:
  - After applying the remediation steps, I will conduct follow-up scans using both Nessus and Nmap. These scans will verify whether the vulnerabilities have been successfully mitigated.
  - The effectiveness of the remediation efforts will be demonstrated by comparing the results of the initial and post-remediation scans.

#### Conclusion:

This project will provide a thorough demonstration of the vulnerability management lifecycle, from initial identification to final remediation. By using Nmap and Nessus on a Kali Linux Virtual Machine to scan a Windows 10 host machine, and employing Action1 for remediation within the host, I will effectively show how to secure a system against potential threats. The final rescan will confirm the success of the remediation process, ensuring that the host machine is better protected against attacks.