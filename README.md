# 🛡️ Windows Authentication Log Analysis Lab

## 📌 Overview

This project demonstrates how to analyze authentication activity within a Windows-based Active Directory environment using Event Viewer.

The lab focuses on identifying and interpreting login events to understand how systems log and track user authentication behavior.

---

## 🧱 Lab Environment

| System              | Role                   | IP Address     |
| ------------------- | ---------------------- | -------------- |
| Windows Server 2022 | Domain Controller (DC) | 192.168.56.10  |
| Windows 10 Client   | Domain-joined Machine  | 192.168.100.10 |

* **Platform:** VirtualBox
* **Domain:** lab.local
* **Log Source:** Windows Security Event Log

---

## 🎯 Objectives

* Generate authentication activity within a domain environment
* Identify relevant security events using Event Viewer
* Analyze login behavior using Windows Security logs
* Understand differences between successful and failed authentication events
* Build foundational skills for security monitoring and incident detection

---

## ⚙️ Configuration

### Event Viewer Access

Opened Event Viewer using:

```bash
eventvwr.msc
```

Navigated to:

```plaintext
Windows Logs → Security
```

---

### Event Filtering

* Used **Filter Current Log** to isolate authentication events
* Focused on:

  * Event ID 4624 (successful logon)
  * Event ID 4625 (failed logon)

---

## 🧪 Validation

✔ Authentication events successfully generated from Windows 10 client  
✔ Event ID 4624 (successful logon) identified in Security logs  
✔ Event ID 4625 (failed logon) identified and analyzed  
✔ Log filtering used to isolate relevant security events  
✔ Event details reviewed to extract account and system information  

---

## 📸 Screenshots

Screenshots available in the [screenshots directory](notes/screenshots).

---

## 📚 Skills Demonstrated

* Windows Event Viewer navigation and usage
* Security log analysis (Event ID 4624 / 4625)
* Understanding authentication workflows in Active Directory
* Filtering and isolating relevant log data
* Interpreting system-generated security events

---

## 🚧 Project Status

* [x] Authentication activity generated
* [x] Security logs accessed and analyzed
* [x] Event filtering implemented
* [x] Key authentication events identified
* [x] Event data interpreted and documented

---

## 🚀 Next Steps

* Integrate centralized logging using SIEM (Splunk)
* Simulate brute-force login attempts and analyze patterns
* Correlate authentication logs across multiple systems
* Develop detection rules for suspicious login activity

---

## 🧠 Key Takeaway

* Developed foundational skills in analyzing authentication logs within a Windows environment
* Gained hands-on experience using Event Viewer to investigate system activity
* Understood how successful and failed logons are recorded and interpreted
* Learned how log visibility depends on system configuration and authentication path
* Established a baseline for transitioning into SIEM-based security monitoring
