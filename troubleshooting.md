# Troubleshooting ProtonVPN on Kali Linux

This file lists common issues you may face while setting up or using ProtonVPN and their fixes.

---

## 🚫 Issue 1: `protonvpn: command not found`
**Cause:** Wrong package or incomplete installation.  
**Fix:**
```bash
sudo apt update
sudo apt install proton-vpn-gnome-desktop -y
````

Then start with:

```bash
protonvpn-app
```

---

## 🚫 Issue 2: Authentication failed (wrong username/password)

**Cause:** Using system login instead of ProtonVPN account.
**Fix:**

* Sign up at [ProtonVPN](https://protonvpn.com) and use those credentials.
* If you forgot password, reset it from ProtonVPN website.

---

## 🚫 Issue 3: Connection stuck / cannot connect to server

**Fix:**

1. Disconnect and try another server.
2. Check your internet connection before VPN.
3. Restart the app:

   ```bash
   pkill protonvpn-app && protonvpn-app
   ```

---

## 🚫 Issue 4: Slow internet speed

**Cause:** Free VPN servers may be overloaded.
**Fix:**

* Switch to a different free server.
* Use a server closer to your location.
* Consider upgrading to ProtonVPN Plus for faster speeds.

---

## 🚫 Issue 5: Error during package installation (externally managed environment)

**Fix:**
Use APT installation instead of pip:

```bash
sudo apt install proton-vpn-gnome-desktop -y
```

---

## 🚫 Issue 6: IP does not change after connecting

**Cause:** VPN not properly initialized.
**Fix:**

1. Disconnect and reconnect.
2. Verify using:

   ```bash
   curl ifconfig.me
   ```

   (should show new VPN IP).

---

## ✅ General Tips

* Always run updates before installation:

  ```bash
  sudo apt update && sudo apt upgrade -y
  ```
* If nothing works, reboot your system and try again.
* Check ProtonVPN status page for server outages.

