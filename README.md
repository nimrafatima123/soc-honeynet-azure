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



