
# Windows Threat Detection & Incident Response Lab Using Splunk and Sysmon

## Overview

This project demonstrates a Security Operations Center (SOC) home lab built using Splunk Enterprise, Sysmon, and Windows Event Logs.

The goal of the project was to simulate attacker behavior, create detections, perform investigations, conduct threat hunting, and document incident response procedures.

---

## Technologies Used

* Splunk Enterprise
* Sysmon
* Windows Event Logs
* PowerShell
* MITRE ATT&CK Framework

---

## Detection Use Cases

### Brute Force Detection

* Event ID: 4625
* MITRE ATT&CK: T1110

### User Account Creation

* Event ID: 4720
* MITRE ATT&CK: T1136.001

### Privilege Escalation

* Event ID: 4732
* MITRE ATT&CK: T1098

### PowerShell Execution

* Sysmon Event ID: 1
* MITRE ATT&CK: T1059.001

### Network Connections

* Sysmon Event ID: 3
* MITRE ATT&CK: T1071

### DNS Queries

* Sysmon Event ID: 22
* MITRE ATT&CK: T1071

---

## Correlation Rule

A correlation rule was created to identify user creation followed by administrator group assignment within a short period of time.

---

## Threat Hunting

Threat hunting queries were developed for:

* PowerShell activity
* Administrative group changes
* DNS activity
* Network connections

---

## Incident Investigations

### Incident 01

Brute Force Login Investigation

### Incident 02

Persistence and Privilege Escalation Investigation

### Incident 03

PowerShell and Network Activity Investigation

---

## Dashboard

The SOC dashboard contains:

* Failed Logins
* User Account Creation
* Privilege Escalation
* PowerShell Activity
* Network Connections
* DNS Queries

---

## Outcome

This project demonstrates SIEM monitoring, detection engineering, threat hunting, dashboard creation, MITRE ATT&CK mapping, and incident response workflows using Splunk and Sysmon.
