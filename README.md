# 🛡️ Windows Authentication Log Analysis

## 📌 Overview

This project demonstrates how to analyze authentication events using Windows Event Viewer within an Active Directory lab environment.

The goal is to identify and interpret login activity to understand how systems log and track user authentication.

---

## 🎯 Objective

* Generate authentication activity from a domain-joined Windows 10 client
* Locate relevant security events in Event Viewer
* Analyze key fields to understand login behavior

---

## 🧱 Lab Environment

* Windows Server 2022 (Domain Controller)
* Windows 10 (Domain-joined client)
* Domain: `lab.local`
* Platform: VirtualBox

---

## ⚔️ Activity Performed

* Performed multiple login attempts using domain credentials
* Generated authentication events from the Windows 10 system
* Observed how authentication activity is recorded in system logs

---

## 🔍 Log Analysis

### Event ID 4624 — Successful Logon

This event indicates a successful authentication attempt.

Key fields analyzed:

* **Account Name** — user who logged in
* **Account Domain** — domain of the user
* **Logon Type** — method of login (interactive or network)
* **Workstation Name** — source machine

---

### Event ID 4625 — Failed Logon

This event indicates a failed authentication attempt.

Key fields analyzed:

* **Account Name**
* **Failure Reason** (e.g., incorrect password)
* **Logon Type**
* **Source Workstation**

> Note: Logging behavior may vary depending on system configuration and authentication path in a lab environment.

---

## 📸 Screenshots

![Authentication Event](/notes/screenshots/02-event-4625.png)
*Example authentication event in Windows Security log*

![Event Details](/notes/screenshots/03-event-details.png)
*Detailed view showing account, domain, and authentication information*

📁 **View all screenshots:** [screenshots directory](notes/screenshots/)

---

## 🧠 Key Takeaways

* Windows logs authentication activity in the Security log
* Event Viewer is essential for investigating system and user behavior
* Authentication events provide insight into login patterns and potential security issues
* Log visibility depends on system configuration and where authentication occurs

---

## 🚀 Skills Demonstrated

* Log analysis using Windows Event Viewer
* Understanding authentication events (4624 / 4625)
* Interpreting security logs in an Active Directory environment
* Troubleshooting logging behavior in a lab setup
