\# 🔥 Windows Firewall Rule Lab – Port 420



\## 📌 Overview



This lab demonstrates how to create an inbound firewall rule using Windows Defender Firewall with Advanced Security.



The objective was to allow traffic on TCP port 420 by creating a rule named \*\*AllowPing\*\*.



---



\## 🎯 Objectives



\* Create an inbound firewall rule

\* Configure protocol and port settings

\* Allow network traffic through a specific port

\* Understand firewall rule behavior



---



\## 🛠️ Tools Used



\* Windows Defender Firewall with Advanced Security

\* Windows Virtual Machine



---



\## ⚙️ Steps Performed



\### 1. Open Firewall Console



Accessed Windows Firewall with Advanced Security.



!\[Step 1](screenshots/step1-firewall-dashboard.png)



---



\### 2. Navigate to Inbound Rules



Selected inbound rules to control incoming traffic.



!\[Step 2](screenshots/step2-inbound-rules.png)



---



\### 3. Create New Rule (Port 420)



Configured a TCP rule for port 420.



!\[Step 3](screenshots/step3-port-420.png)



---



\### 4. Allow Connection



Selected "Allow the connection" and applied to all profiles.



!\[Step 4](screenshots/step4-action-profile.png)



---



\### 5. Final Rule Created



Verified the rule "AllowPing" was successfully created.



!\[Step 5](screenshots/step5-final-rule.png)



---



\## 🧠 Key Concepts



\* \*\*Firewall Rule\*\*: Controls network traffic based on defined criteria

\* \*\*Inbound Traffic\*\*: Incoming connections to a system

\* \*\*Port Filtering\*\*: Allowing or blocking traffic by port number

\* \*\*Security Profiles\*\*: Domain, Private, Public network settings



---



\## 🔐 Security Insight



Opening a port allows external communication into a system. If misconfigured, this can expose services to attackers. Proper firewall configuration is critical for securing systems.



---



\## 🚀 Outcome



Successfully created and verified an inbound firewall rule allowing TCP traffic on port 420.



---



\## 📎 Author



Mozella L. McCoy-Flowers

Cybersecurity \& Digital Forensics Student

Virginia State University



