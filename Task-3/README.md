# Task 3: Basic Vulnerability Scan Using Nessus

## Objective
Perform a basic vulnerability assessment on a local Kali Linux system using Nessus Essentials to identify security weaknesses and document findings.

---

## Environment
- OS: Kali Linux
- Scanner: Nessus Essentials
- Target: 127.0.0.1
- Scan Type: Basic Network Scan

---

## Tools Used
- Nessus Essentials
- Kali Linux
- Firefox Browser

---

## Installation & Setup

wget https://www.tenable.com/downloads/api/v2/pages/nessus/files/Nessus-10.x.x-debian10_amd64.deb  
sudo dpkg -i Nessus-10.x.x-debian10_amd64.deb  
sudo apt --fix-broken install -y  
sudo systemctl start nessusd  
sudo systemctl enable nessusd
