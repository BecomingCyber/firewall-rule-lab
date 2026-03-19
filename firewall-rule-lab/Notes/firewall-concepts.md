\# 🔐 Firewall Concepts – Study Notes



\## 📌 Overview



This document explains the key concepts behind firewall rules and how they are used to control network traffic. These concepts are foundational for cybersecurity roles such as SOC Analyst, Network Security Engineer, and Incident Responder.



---



\## 🧠 What is a Firewall?



A firewall is a security system that monitors and controls incoming and outgoing network traffic based on predefined security rules.



\### 🔎 Purpose:



\* Prevent unauthorized access

\* Allow legitimate traffic

\* Enforce network security policies



---



\## 🔄 Types of Traffic



\### 📥 Inbound Traffic



\* Traffic coming \*\*into\*\* a system

\* Example: A remote computer trying to connect to your machine



\### 📤 Outbound Traffic



\* Traffic going \*\*out of\*\* a system

\* Example: Your system connecting to a website



---



\## ⚙️ Firewall Rules



A firewall rule defines how traffic should be handled.



\### 🧩 Key Components:



| Component | Description                                         |

| --------- | --------------------------------------------------- |

| Direction | Inbound or Outbound                                 |

| Protocol  | TCP, UDP, ICMP                                      |

| Port      | Specific communication channel (e.g., 80, 443, 420) |

| Action    | Allow or Block                                      |

| Profile   | Domain, Private, Public                             |



---



\## 🌐 Ports Explained



Ports are logical communication endpoints used by applications.



\### 📌 Common Ports:



| Port | Protocol | Purpose                     |

| ---- | -------- | --------------------------- |

| 80   | TCP      | HTTP (Web Traffic)          |

| 443  | TCP      | HTTPS (Secure Web Traffic)  |

| 22   | TCP      | SSH (Remote Access)         |

| 3389 | TCP      | RDP (Remote Desktop)        |

| 420  | TCP      | Custom/Application-specific |



---



\## 🔗 Protocols



\### TCP (Transmission Control Protocol)



\* Reliable, connection-based

\* Used for web, email, file transfers



\### UDP (User Datagram Protocol)



\* Faster, connectionless

\* Used for streaming, gaming



\### ICMP (Internet Control Message Protocol)



\* Used for diagnostics (e.g., ping)



---



\## 🚦 Firewall Actions



\### ✅ Allow



\* Permits traffic to pass through



\### ❌ Block



\* Denies traffic completely



---



\## 🏠 Network Profiles



Firewall rules can apply to different environments:



| Profile | Description                             |

| ------- | --------------------------------------- |

| Domain  | Corporate network                       |

| Private | Trusted home network                    |

| Public  | Untrusted network (e.g., Wi-Fi at café) |



---



\## ⚠️ Security Risks



Improper firewall configuration can lead to:



\* Open ports exposing services

\* Unauthorized remote access

\* Increased attack surface

\* Data exfiltration



---



\## 🧠 Real-World SOC Insight



Attackers often:



\* Scan for open ports using tools like \*\*Nmap\*\*

\* Target exposed services (e.g., RDP, SSH)

\* Exploit misconfigured firewall rules



Defenders must:



\* Limit open ports

\* Monitor traffic

\* Apply least privilege principles



---



\## 🧪 Lab Connection



In this lab, an inbound rule was created to:



\* Allow TCP traffic on port 420

\* Apply to all network profiles

\* Demonstrate controlled access through firewall configuration



---



\## 🛡️ Best Practices



\* Only open required ports

\* Use "Block" by default where possible

\* Regularly audit firewall rules

\* Log and monitor firewall activity

\* Apply least privilege access



---



\## 🎯 Key Takeaways



\* Firewalls are a first line of defense in network security

\* Rules define how traffic is handled

\* Ports and protocols determine communication behavior

\* Misconfiguration can create serious vulnerabilities



---



\## 📎 Author Notes



These concepts align with:



\* CompTIA Security+ (SY0-701)

\* SOC Analyst responsibilities

\* Real-world network defense strategies



