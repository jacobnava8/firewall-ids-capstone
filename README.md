# 🔥 Firewall & IDS Capstone Project

## 📌 Overview
This project demonstrates how to configure and test a **Firewall** and **Intrusion Detection System (IDS)** to improve network security.  
The setup includes firewall rules to control traffic between trusted/untrusted networks and IDS rules to log and detect suspicious activity.

---

## 📂 Project Structure
📂 firewall-ids-capstone
├── configs/ # Firewall and IDS configuration files
├── logs/ # Sample IDS logs showing detected attacks
├── docs/ # Documentation or architecture diagrams
└── README.md


---

## 🚀 How to Use
1. Install an IDS such as **Snort** or **Security Onion**.  
2. Load configuration files from the `configs/` directory.  
3. Start the IDS and monitor logs in `logs/`.  
4. Apply provided firewall rules (Linux iptables or Windows Firewall).  
5. Simulate malicious traffic (e.g., FTP attempts from untrusted network) to test detection/blocking.  

---

## 🛠️ Tech Stack
- IDS/IPS: **Snort**, Security Onion  
- Firewalls: **iptables**, Windows Firewall  
- Networking: TCP/IP, DMZ setup, FTP traffic control  

---

## 📊 Results
- Successfully logged suspicious traffic (FTP attempts) using IDS rules  
- Implemented firewall rules to block malicious connections from untrusted sources  
- Improved visibility into network attacks through centralized logging  
