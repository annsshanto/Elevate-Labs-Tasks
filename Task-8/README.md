# VPN Setup and Privacy Verification on Kali Linux

## Objective
Understand the role of VPNs in protecting privacy and securing communication by encrypting traffic and masking IP address.

---

## Tools Used
- Kali Linux 2025
- ProtonVPN (Free Tier)

---

## Step 1: Update System

sudo apt update && sudo apt upgrade -y
Step 2: Install Required Packages
sudo apt install -y curl gpg
Step 3: Add ProtonVPN GPG Key
curl -fsSL https://repo.protonvpn.com/debian/public_key.asc | sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/protonvpn.gpg

Verify key exists:

ls /etc/apt/trusted.gpg.d/protonvpn.gpg
Step 4: Add ProtonVPN Repository
echo "deb https://repo.protonvpn.com/debian stable main" | sudo tee /etc/apt/sources.list.d/protonvpn-stable.list
Step 5: Update Repository List
sudo apt update
Step 6: Install ProtonVPN Application
sudo apt install -y proton-vpn-gnome-desktop
Step 7: Launch ProtonVPN
protonvpn-app
Step 8: Login to ProtonVPN

Login using ProtonVPN free account.

Screenshot:

screenshots/login.png
Step 9: Connect to VPN Server

Select a free server and click Quick Connect.

Screenshot:

screenshots/connected.png
Step 10: Check IP Address Before VPN
curl ifconfig.me

Screenshot:

screenshots/ip-before.png
Step 11: Check IP Address After VPN
curl ifconfig.me

Screenshot:

screenshots/ip-after.png
Step 12: Verify Encrypted Browsing

Open HTTPS website:

firefox https://example.com

Confirm lock icon in address bar.

Screenshot:

screenshots/https-lock.png
Step 13: Speed Test Without VPN

Disconnect VPN.

speedtest-cli

Screenshot:

screenshots/speed-no-vpn.png
Step 14: Speed Test With VPN

Connect VPN.

speedtest-cli

Screenshot:

screenshots/speed-vpn.png
Step 15: Disconnect VPN

Click Disconnect inside ProtonVPN app.

Screenshot:

screenshots/disconnected.png
Observations

Public IP changes after VPN connection.

HTTPS websites show encrypted connection.

Internet speed decreases slightly when VPN is enabled.

VPN Benefits

Hides real IP address

Encrypts internet traffic

Protects data on public Wi-Fi

Improves privacy

VPN Limitations

Reduced speed

Free servers limited

Must trust VPN provider

Conclusion

VPNs help secure communication and improve privacy by encrypting data and masking the user’s identity.
