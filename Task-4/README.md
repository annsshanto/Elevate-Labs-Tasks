# Task 4 – Setup and Use a Firewall on Kali Linux (UFW)

## Objective

Configure and test basic firewall rules to allow or block network traffic using UFW (Uncomplicated Firewall) on Kali Linux.

---

## Tools Used

- Kali Linux  
- UFW (Uncomplicated Firewall)  
- Telnet Client  

---

## Step 1: Install and Enable UFW

sudo apt update  
sudo apt install ufw -y  
sudo ufw enable  
sudo ufw status  

![UFW enabled status](screenshots/ufw_enable.png)  

Firewall status shows **active**, confirming UFW is enabled.

---

## Step 2: View Current Firewall Rules

sudo ufw status numbered  

![UFW status numbered](screenshots/ufw_status_numbered)  

Displays all existing firewall rules with numbering.

---

## Step 3: Block Telnet Port (23)

sudo ufw deny 23  
sudo ufw status numbered  

![UFW telnet block](screenshots/telnet_block.png)  

This rule blocks inbound traffic on port 23 (Telnet).







  

