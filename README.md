# 🔥 Firewall & IDS Capstone Project

## 📌 Overview
This project was conducted as a continuation of client network security improvements.  
The goal was to **identify and log attacks** against web and production servers by installing an **Intrusion Detection/Prevention System (IDS/IPS)** and configuring **firewall rules**.  
The solution was implemented on **pfSense** with **Snort** to detect, alert, and block malicious traffic:contentReference[oaicite:0]{index=0}.

---

## 📂 Project Structure
📂 firewall-ids-capstone

├── configs/ # pfSense firewall rules, Snort configs

├── logs/ # Sample IDS alerts and logs

├── docs/ # Reports, screenshots, diagrams

└── README.md

---

## 🛠️ Tasks Performed
- **System Preparation**
  - Enabled **Network Adapter 4** on pfSense to allow internet access  
  - Updated **pfSense** to the latest version

- **Snort Installation & Setup**
  - Installed **Snort** from pfSense Package Manager  
  - Enabled **Snort VRT** rules with Oinkmaster code  
  - Added **Untrusted, Trusted, and DMZ interfaces** under Snort configuration

- **Firewall Configuration**
  - Created firewall rules to **block FTP traffic** from the Untrusted network to the DMZ

- **Custom IDS Rules & Alerts**
  - Configured Snort to generate alerts for:  
    - Xmas scan from Kali (Untrusted → 10.200.0.12)  
    - FTP attempts from Kali (Untrusted → 10.200.0.12)  
    - Nmap ping sweep from Kali (Untrusted → 10.200.0.12)

---

## 🚀 How to Use
1. Deploy **pfSense** in a VM or hardware firewall.  
2. Enable required network adapters and update pfSense.  
3. Install **Snort** via Package Manager.  
4. Configure Snort rules using Oinkmaster code.  
5. Assign interfaces (Untrusted, Trusted, DMZ) in Snort.  
6. Apply provided firewall rules in `configs/`.  
7. Simulate malicious traffic (Nmap, Xmas scans, FTP attempts) from Kali Linux.  
8. Review alerts and logs in `logs/`.  

---

## 🛠️ Tech Stack
- **Firewall**: pfSense  
- **IDS/IPS**: Snort  
- **Tools**: Nmap, Kali Linux (Xmas Scan, FTP attempt, Ping Sweep)  
- **Protocols**: FTP, TCP/IP, DMZ segmentation  

---

## 📊 Results
- ✅ **Suspicious traffic logged** in Snort for Xmas scans, FTP attempts, and Nmap sweeps  
- ✅ **Firewall blocked FTP traffic** from Untrusted → DMZ
- ✅ Enhanced visibility into attacks on production/web servers  
- ✅ Delivered a layered defense with **IDS detection** + **firewall enforcement**  

---

⚠️ **Disclaimer**: This project was completed in a **controlled lab environment**. The tools and configurations are for educational and authorized use only.  
