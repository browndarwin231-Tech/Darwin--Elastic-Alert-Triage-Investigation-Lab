# Darwin--Elastic-Alert-Triage-Investigation-Lab

## Overview

This project demonstrates a complete Security Operations Center (SOC) investigation using Elastic Security (Kibana) within the TryHackMe **Alert Triage With Elastic** lab.

The investigation covers multiple attack scenarios, including:

- Web attack analysis
- HTTP POST and GET request investigation
- Windows Security Event Log analysis
- Administrator logon investigation
- Sysmon Process Creation events
- Security Group Management events
- PowerShell Script Block Logging (Event ID 4104)
- Privilege Escalation investigation

Throughout the lab, Elastic Discover was used to search, filter, and correlate logs to identify malicious activity and answer investigation questions.

---

## Skills Demonstrated

- Elastic Security
- Kibana Discover
- Security Monitoring
- Threat Hunting
- Windows Event Log Analysis
- Sysmon Investigation
- Event Correlation
- PowerShell Analysis
- Privilege Escalation Detection
- Security Event Investigation
- Blue Team Operations
- SOC Alert Triage

---

## Technologies Used

- Elastic Stack
- Kibana Discover
- Elastic Security
- Sysmon
- Windows Security Logs
- PowerShell
- TryHackMe
- Windows Server
- KQL-style Searching

---

# Investigation Walkthrough

## 1. Lab Introduction

**Screenshot**

`01-Alert-Triage-With-Elastic-Introduction.png`

Introduces the Alert Triage With Elastic room and investigation objectives.

---

## 2. Kibana Discover Interface

**Screenshot**

`02-Kibana-Discover-Interface.png`

Opened Kibana Discover and became familiar with the investigation interface.

---

## 3. Web Logs Loaded

**Screenshot**

`03-Kibana-Weblogs-Loaded.png`

Verified log ingestion and confirmed available web server events.

---

## 4. Investigating Web Attacks (POST Requests)

**Screenshot**

`04-Investigating-Web-Attacks-POST-Requests.png`

Filtered suspicious POST requests to identify malicious web activity.

---

## 5. GET Request Investigation

**Screenshot**

`05-Elastic-GET-Requests-ErrorEE-Investigation.png`

Investigated suspicious GET requests and server errors.

---

## 6. Command Execution Investigation

**Screenshot**

`07-Elastic-Command-Execution-Old-New.png`

Compared process execution events to identify suspicious command activity.

---

## 7. Web Attack Investigation Results

**Screenshot**

`08-Elastic-Web-Attack-Investigation-Answers.png`

Completed the investigation questions related to the web attack scenario.

---

## 8. Administrator Logon Investigation

**Screenshot**

`09-Elastic-Administrator-Logon-Event-4624.png`

Investigated Windows Security Event ID 4624 to identify successful Administrator logon activity.

---

## 9. Task 4 Investigation Answers

**Screenshot**

`10-Task4-Final-Answers.png`

Completed Task 4 by correlating Windows Security logs and Sysmon events.

---

## 10. Command-Line Investigation

**Screenshot**

`11-Elastic-Command-Line-Investigation-Query.png`

Built a search query to investigate suspicious command-line execution.

---

## 11. Sysmon Process Investigation

**Screenshot**

`11-Elastic-Sysmon-ProcessID-964.png`

Investigated Sysmon Process Create events and identified Process ID **964** associated with suspicious activity.

---

## 12. Security Group Management Investigation

**Screenshot**

`13-Elastic-Security-Group-Management-Investigation.png`

Correlated Windows Event ID 4732 with Sysmon events to identify modifications to security-enabled local groups.

---

## 13. PowerShell Investigation

**Screenshot**

`14-Elastic-PowerShell-4104-Remote-Command-Investigation.png`

Reviewed PowerShell Script Block Logging (Event ID 4104) to identify administrative commands including:

- whoami
- whoami /priv
- net localgroup Administrators
- net group "Domain Admins" /domain

This activity demonstrated privilege enumeration and possible privilege escalation.

---

# What I Learned

During this project I learned how to:

- Investigate security alerts using Elastic Security
- Search Windows Security Event Logs
- Analyze Sysmon Process Create events
- Detect privilege escalation behavior
- Investigate PowerShell activity
- Correlate multiple log sources
- Perform SOC alert triage
- Identify suspicious administrative activity
- Build effective search queries in Kibana Discover

---

# Career Skills Demonstrated

- Security Monitoring
- SIEM Investigation
- Elastic Security
- Windows Event Analysis
- Threat Hunting
- Blue Team Investigation
- Incident Response
- Log Correlation
- Privilege Escalation Detection
- SOC Tier 1 Analysis

---

# Author

**Darwin Brown JR**

Aspiring SOC Tier 1
