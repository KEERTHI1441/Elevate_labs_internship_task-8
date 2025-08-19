# VPN Setup & Privacy Protection (Task 8)

## 📌 Objective
The goal of this task was to understand the role of **VPNs** (Virtual Private Networks) in protecting privacy and enabling secure communication.

---

## 🛠️ Tools Used
- **ProtonVPN (Free Tier)**
- **Kali Linux**
- Verification sites: [whatismyipaddress.com](https://whatismyipaddress.com)

---

## 🚀 Setup Steps
1. Added ProtonVPN repository to Kali Linux.  
2. Installed ProtonVPN GUI client:
   ```bash
   sudo apt install proton-vpn-gnome-desktop -y
````

3. Launched app:

   ```bash
   protonvpn-app
   ```
4. Logged in using ProtonVPN account credentials.
5. Connected to a nearby VPN server.
6. Verified new IP on [whatismyipaddress.com](https://whatismyipaddress.com).
7. Browsed securely to confirm traffic was encrypted.
8. Disconnected and compared browsing speed & IP before/after VPN.

---

## 📷 Deliverables

* **Connection screenshot** showing successful ProtonVPN connection.
* **IP verification screenshot** (before and after connecting).

---

## 🔒 VPN Benefits

* Hides real IP and location.
* Encrypts all internet traffic.
* Prevents tracking and enhances online privacy.
* Protects when using public Wi-Fi.

---

## ⚠️ Limitations

* Free VPN servers may be slower.
* Limited number of server locations in free tier.
* VPNs protect traffic, but do not guarantee full anonymity.

---

## 🎯 Outcome

* Successfully set up and tested ProtonVPN on Kali Linux.
* Verified that IP address changes when connected to VPN.
* Gained hands-on experience with **VPNs as a privacy tool**.
