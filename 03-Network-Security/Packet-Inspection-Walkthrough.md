# 🛡️ Cybersecurity Incident Report: Network Traffic Analysis

> [!NOTE]
> **Portfolio Project Disclaimer:**  
> This incident report was developed as part of practical coursework demonstrating network traffic analysis, packet inspection (`tcpdump`), and troubleshooting critical DNS/network infrastructure failures.

---

## 📌 Executive Summary

* **Target URL:** `www.yummyrecipesforme.com`
* **Incident Timestamp:** `13:24:32.192571`
* **Affected Service / Port:** DNS Server (`UDP Port 53`)
* **Primary Symptom:** Host unreachable / Connection timeout for end users
* **Investigation Tools Used:** Web Browser reproduction, `tcpdump` packet capture
* **Root Cause Assessment:** Unresponsive DNS server likely resulting from a misconfigured firewall rule or an ongoing Denial of Service (DoS) attack.

---

## Part 1: Traffic Analysis & Problem Summary (DNS & ICMP)

### 1. Protocol Interaction Overview
* **UDP (User Datagram Protocol):** When client browsers navigated to `www.yummyrecipesforme.com`, standard DNS queries were initiated over UDP to resolve the domain name to its corresponding IP address.
* **ICMP (Internet Control Message Protocol):** Because the target DNS server failed to acknowledge the queries, the network generated ICMP error messages indicating communication failures back to the client.

### 2. Packet Capture & Error Details
* **Observed Error Message:**  
  ```text
  ICMP 203.0.113.2 udp port 53 unreachable
