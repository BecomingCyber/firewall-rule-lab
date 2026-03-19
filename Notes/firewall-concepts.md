> 🔙 Back to lab: See the main walkthrough and portfolio context in `README.md` at the root of this repo.

# 🔐 Firewall Concepts – Study Notes

## 📌 Overview

This document explains the key concepts behind firewall rules and how they are used to control network traffic. These concepts are foundational for cybersecurity roles such as SOC Analyst, Network Security Engineer, and Incident Responder.

---

## 🧠 What is a Firewall?

A firewall is a security system that monitors and controls incoming and outgoing network traffic based on predefined security rules.

### 🔎 Purpose

- Prevent unauthorized access  
- Allow legitimate traffic  
- Enforce network security policies  

---

## 🔄 Types of Traffic

### 📥 Inbound Traffic

- Traffic coming **into** a system  
- Example: A remote computer trying to connect to your machine  

### 📤 Outbound Traffic

- Traffic going **out of** a system  
- Example: Your system connecting to a website  

---

## ⚙️ Firewall Rules

A firewall rule defines how traffic should be handled.

### 🧩 Key Components

| Component | Description                                           |
|----------|-------------------------------------------------------|
| Direction| Inbound or Outbound                                  |
| Protocol | TCP, UDP, ICMP                                       |
| Port     | Communication channel (e.g., 80, 443, 420)           |
| Action   | Allow or Block                                       |
| Profile  | Domain, Private, Public                              |

---

## 🌐 Ports Explained

Ports are logical communication endpoints used by applications.

### 📌 Common Ports

| Port | Protocol | Purpose                     |
|------|----------|-----------------------------|
| 80   | TCP      | HTTP (Web Traffic)          |
| 443  | TCP      | HTTPS (Secure Web Traffic)  |
| 22   | TCP      | SSH (Remote Access)         |
| 3389 | TCP      | RDP (Remote Desktop)        |
| 420  | TCP      | Custom / Lab-specific Port  |

---

## 🔗 Protocols

### TCP (Transmission Control Protocol)

- Reliable, connection-based  
- Used for web, email, file transfers  

### UDP (User Datagram Protocol)

- Faster, connectionless  
- Used for streaming, gaming  

### ICMP (Internet Control Message Protocol)

- Used for diagnostics (for example, ping)  

---

## 🚦 Firewall Actions

### ✅ Allow

- Permits traffic to pass through  

### ❌ Block

- Denies traffic completely  

---

## 🏠 Network Profiles

Firewall rules can apply to different environments:

| Profile | Description                               |
|---------|-------------------------------------------|
| Domain  | Corporate / domain-joined network        |
| Private | Trusted home or office network           |
| Public  | Untrusted network (for example, café Wi‑Fi) |

---

## ⚠️ Security Risks

Improper firewall configuration can lead to:

- Open ports exposing services  
- Unauthorized remote access  
- Increased attack surface  
- Data exfiltration  

---

## 🧠 Real-World SOC Insight

Attackers often:

- Scan for open ports using tools like **Nmap**  
- Target exposed services (for example, RDP, SSH)  
- Exploit misconfigured firewall rules  

Defenders must:

- Limit open ports  
- Monitor traffic and firewall logs  
- Apply least privilege principles  

---

## 🧪 Lab Connection

In this lab, you implemented these concepts on a real Windows host by:

- Creating an **inbound** rule named `AllowPing`.  
- Allowing **TCP traffic on port 420** to reach the system.  
- Applying the rule to **all network profiles** (Domain, Private, Public).  
- Verifying that the `AllowPing` rule was enabled and allowed traffic using:
  - The Windows Defender Firewall console.
  - PowerShell (`Get-NetFirewallRule`) to confirm `Enabled = True` and `Action = Allow`.
  - Network tests targeting TCP port 420 from another system.

This mirrors how a SOC analyst or blue-team engineer would validate that a host-based firewall change is correctly implemented and documented.

---

## 🛡️ Best Practices

- Only open required ports  
- Use “Block” by default where possible  
- Regularly audit firewall rules  
- Log and monitor firewall activity  
- Apply least privilege access  

---

## 🎓 Exam Alignment

These concepts support:

- **CompTIA Security+ (SY0‑701)**
  - Secure network design and segmentation  
  - Host-based security controls  
  - Securing remote access services (RDP, SSH)  

- **CompTIA CySA+ (CS0‑003)**
  - Interpreting firewall and network logs  
  - Identifying suspicious inbound/outbound traffic  
  - Validating and hardening firewall rule configurations  