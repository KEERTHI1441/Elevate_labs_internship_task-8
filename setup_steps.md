````markdown
# VPN Setup Guide (ProtonVPN on Kali Linux)

## 🔧 Prerequisites
- Kali Linux system
- Internet connection
- ProtonVPN account (Free Tier or Paid)

---

## 📥 Installation Steps

1. **Update system packages**
   ```bash
   sudo apt update && sudo apt upgrade -y
````

2. **Add ProtonVPN repository**
   A repo entry is created at:

   ```
   /etc/apt/sources.list.d/protonvpn.list
   ```

   Example:

   ```
   deb [arch=amd64 signed-by=/etc/apt/trusted.gpg.d/protonvpn.asc] https://repo.protonvpn.com/debian stable main
   ```

3. **Install ProtonVPN client**

   ```bash
   sudo apt install proton-vpn-gnome-desktop -y
   ```

4. **Launch ProtonVPN app**

   ```bash
   protonvpn-app
   ```

5. **Login with ProtonVPN account**

   * Enter username & password created from [ProtonVPN Signup](https://protonvpn.com).

6. **Connect to a server**

   * Choose the nearest server or any preferred location.
   * Wait for the VPN connection to be established.

---

## ✅ Verification Steps

1. Check your IP before VPN:

   * Visit [whatismyipaddress.com](https://whatismyipaddress.com).
2. Connect to VPN.
3. Check IP again (should be different).
4. Browse securely to confirm encrypted traffic.

---

## 📌 Notes

* Free tier has limited server locations.
* Use **Disconnect** option in the client when finished.

```
```
