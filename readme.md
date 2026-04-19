# Centralized Windows Log Analysis  
### Splunk · Windows Event Logs

## Objective

Understand how Windows Security logs are collected, centralized, and analyzed in a SIEM environment.

---

## Scenario

Windows authentication events (successful and failed logins) were collected from a local system and forwarded to a central Splunk server for analysis.

---

## What I Did

- Installed and configured Splunk Enterprise on a Linux VM  
- Installed Splunk Universal Forwarder on a Windows system  
- Forwarded Windows Security logs (Event ID 4624 and 4625) to Splunk  
- Verified log ingestion over TCP port 9997  
- Queried authentication events using Splunk searches  

---

## Analysis

- Compared successful vs failed login events  
- Identified patterns of repeated failed logins  
- Observed how authentication activity can be monitored centrally instead of locally  

---

## Why This Matters

- Centralized logging is essential for monitoring multiple systems  
- Authentication events provide key indicators of suspicious activity  
- Enables analysts to detect abnormal login behavior across environments  

---

## Skills Demonstrated

- SIEM setup and configuration (Splunk)  
- Log forwarding and ingestion  
- Windows Event Log analysis  
- Basic authentication monitoring  
