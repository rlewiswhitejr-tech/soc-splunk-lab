# Splunk Home SOC Lab: Windows Endpoint Monitoring

**Author:** Ronald White Jr.  
**Project Type:** Home SOC / SIEM Portfolio Lab  
**Tools:** Splunk Enterprise, Splunk Universal Forwarder, Windows Event Logs, Sysmon  
**Focus Areas:** Endpoint monitoring, brute-force detection, PowerShell activity, malware simulation, SOC triage, incident reporting

## Executive Summary

This project demonstrates a practical home SOC lab built with Splunk. The lab collects Windows security telemetry, analyzes suspicious endpoint activity, and presents findings through dashboards, SPL searches, detection rules, and incident writeups.

The goal is to show real SOC analyst skills, including:

- Installing and configuring a SIEM
- Ingesting Windows endpoint logs
- Creating detection searches
- Investigating suspicious activity
- Building dashboards for leadership and analysts
- Writing incident reports based on observable evidence

## Lab Architecture

```text
Windows Endpoint
   |
   |  Windows Event Logs + Sysmon Logs
   v
Splunk Universal Forwarder
   |
   |  TCP Forwarding
   v
Splunk Enterprise Indexer/Search Head
   |
   v
SOC Dashboard + SPL Detection Searches
```

## Data Sources

| Source | Purpose |
|---|---|
| Windows Security Logs | Login activity, failed logons, account events |
| Windows PowerShell Logs | Script execution and command-line activity |
| Sysmon Logs | Process creation, network connections, file activity |
| Splunk Internal Logs | Forwarder/indexer health and ingestion status |

## SOC Use Cases Included

1. Brute-force login detection
2. Suspicious PowerShell execution
3. New process execution monitoring
4. Possible malware execution behavior
5. Endpoint visibility dashboard
6. Incident triage documentation

## Portfolio Value

This lab is designed to show recruiters and hiring managers that I can move beyond theory and build a working SOC environment. It reflects hands-on skills in SIEM operations, endpoint monitoring, log analysis, detection engineering, and incident response documentation.
