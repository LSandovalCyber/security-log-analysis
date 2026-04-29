# Windows Authentication Log Analysis Notes

## 🧠 Overview
This lab demonstrates how to identify and analyze authentication events using Windows Event Viewer.

## 📂 Log Location
- Opened Event Viewer using: eventvwr.msc
- Navigated to:
  Windows Logs → Security

## 🔍 Event Identification
- Located authentication-related events in the Security log
- Focused on:
  - Event ID 4624 (successful logon)
  - Event ID 4625 (failed logon)

## 🧪 Activity Performed
- Attempted multiple logins using domain credentials
- Generated authentication events from Windows 10 client
- Observed how events are recorded in system logs

## 🔎 Event Analysis

### Event ID 4624 — Successful Logon
- Indicates a successful authentication attempt
- Key fields:
  - Account Name (user)
  - Account Domain
  - Logon Type
  - Workstation Name

### Event ID 4625 — Failed Logon
- Indicates a failed authentication attempt
- Common failure reason:
  - Incorrect password
- Key fields:
  - Account Name
  - Failure Reason
  - Logon Type
  - Source Workstation

## 🧠 Key Learning Points
- Authentication events are stored in the Security log
- Event Viewer is a primary tool for investigating system activity
- Successful and failed logons provide insight into user behavior
- Logging behavior can vary depending on system configuration and authentication path
