# soc-honeynet-azure
## ***INTRODUCTION***

This project builds a secure cybersecurity lab in Microsoft Azure that simulates real-world attacks using intentionally vulnerable Windows and Linux virtual machines. The environment integrates a honeynet to attract threats, while Microsoft Sentinel and Defender for Cloud monitor, detect, and respond to malicious activity. The setup demonstrates live log collection, threat detection with KQL queries, incident response workflows, and cloud security best practices — all in a safe, isolated lab.

## ***CLOUD HONEYNET + SOC WORKFLOW :***


![image](https://github.com/user-attachments/assets/4f2d77b6-a2bb-4568-b8d9-7d24022d8ea4)


 ## ***TOOLS & TECHNOLOGIES USED :***
 
- **Microsoft Azure:** Cloud platform hosting the entire lab environment.

- **Windows & Linux Virtual Machines:** Deployed with open inbound rules to simulate real attack surfaces.

- **Microsoft Sentinel:** For centralized log collection, correlation, custom detection rules, and security workbooks.

- **Microsoft Defender for Cloud:** For continuous security posture management, vulnerability detection, and recommendations.

- **SQL Server:** Installed on the Windows VM to generate authentication logs and simulate database attack scenarios.

- **Network Security Groups (NSGs):** Configured to intentionally expose the environment to external threats.

- **Log Analytics Workspace:** To store and query security logs.

- **Kusto Query Language (KQL):** Used to write queries for analyzing logs, detecting threats, and visualizing attack patterns.

- **Geo-IP Watchlists:** Imported to correlate attacker IPs with their geographical origins

## ***Attack Maps Before Hardening / Security Controls***

![Screenshot 2025-07-09 104423](https://github.com/user-attachments/assets/ece62d03-7ebd-44e1-add9-fedacf7734db)

![Screenshot 2025-07-09 104634](https://github.com/user-attachments/assets/28965927-0d3d-49f1-9ff5-4ef00586faf4)

![Screenshot 2025-07-09 105008](https://github.com/user-attachments/assets/015a56df-6664-4242-bffa-a6ecb73c8474)


## ***Attack Maps After Hardening / Security Controls***

![Screenshot 2025-07-09 104743](https://github.com/user-attachments/assets/b528f256-61e3-46eb-9afb-4bbf693e8fed)

Since no malicious activity occurred during the 24 hours after hardening, all map queries produced no results.

## ***Metrics Before Hardening / Security Controls :***

The following table shows the metrics we measured in our insecure environment for 24 hours:

| Metric                   | Count
| ------------------------ | -----
| SecurityEvent            | 3423
| Syslog                   | 1659
| SecurityAlert            | 6
| SecurityIncident         | 1
| AzureNetworkAnalytics_CL | 374

## ***Metrics After Hardening / Security Controls :***

The following table shows the metrics we measured in our environment for another 24 hours, but after applying security controls:


| Metric                   | Count
| ------------------------ | -----
| SecurityEvent            | 1531
| Syslog                   | 0
| SecurityAlert            | 0
| SecurityIncident         | 0
| AzureNetworkAnalytics_CL | 0

## ***RESULTS :***

| Metric                   | Percentage Change After Applying Security Controls
| ------------------------ | -----
| SecurityEvent            | 55.27%
| Syslog                   | 100%
| SecurityAlert            | 100%
| SecurityIncident         | 100%
| AzureNetworkAnalytics_CL | 100%

## ***SUMMARY :***

In this project, I designed and built a live Security Operations Center (SOC) and honeynet using Microsoft Azure. I deployed intentionally vulnerable Windows and Linux virtual machines to attract real attack attempts and generate security data. Using Microsoft Sentinel, Defender for Cloud, and Kusto Query Language (KQL), I collected logs, created custom detection rules, visualized threats, and practiced incident response just like a real SOC team would. This project shows how cloud security tools can be combined to safely simulate attacks, detect threats, and build practical cybersecurity skills in a controlled lab environment.


