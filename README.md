# Xray Core Script Guide

## How to Use the Script

The script was developed and tested on **Ubuntu 22 x64** and **Ubuntu 24 x64**.  
On other operating systems it may not work correctly.  

To download and run the script, use this command:

```sh
wget -qO- https://raw.githubusercontent.com/x-Taiho-x/xray-core-script/refs/heads/main/xray-install | bash
```

---

## User Management Commands

**Show the list of all clients:**

```sh
userlist
```

**Show the link and QR code for connecting the main user:**

```sh
mainuser
```

**Create a new user:**

```sh
newuser
```

**Delete a user:**

```sh
rmuser
```

**Create a connection link:**

```sh
sharelink
```

A file called `help` will be created in the user’s home directory — it contains tips and descriptions of the commands.  
You can view it with the following command (must be run from the user’s home directory):

```sh
cat help
```

---

## Useful Links

- [X-ray Core project on GitHub](https://github.com/XTLS/Xray-core)  
- [Official documentation](https://xtls.github.io/en/)  

---

## Clients for Connection

### Windows
- [v2rayN](https://github.com/2dust/v2rayN)  
- [Furious](https://github.com/LorenEteval/Furious)  
- [Invisible Man - Xray](https://github.com/InvisibleManVPN/InvisibleMan-XRayClient)  

### Android
- [v2rayNG](https://github.com/2dust/v2rayNG)  
- [X-flutter](https://github.com/XTLS/X-flutter)  
- [SaeedDev94/Xray](https://github.com/SaeedDev94/Xray)  

### iOS & macOS arm64
- [Streisand](https://apps.apple.com/app/streisand/id6450534064)  
- [Happ](https://apps.apple.com/app/happ-proxy-utility/id6504287215)  
- [OneXray](https://github.com/OneXray/OneXray)  

### macOS arm64 & x64
- [V2rayU](https://github.com/yanue/V2rayU)  
- [V2RayXS](https://github.com/tzmax/V2RayXS)  
- [Furious](https://github.com/LorenEteval/Furious)  
- [OneXray](https://github.com/OneXray/OneXray)  

### Linux
- [Nekoray](https://github.com/MatsuriDayo/nekoray)  
- [v2rayA](https://github.com/v2rayA/v2rayA)  
- [Furious](https://github.com/LorenEteval/Furious)  

---

## Uninstall Instructions

If you need to uninstall, use these commands:

```sh
bash -c "$(curl -L https://github.com/XTLS/Xray-install/raw/main/install-release.sh)" @ remove
rm /usr/local/etc/xray/config.json
rm /usr/local/etc/xray/.keys
rm /usr/local/bin/userlist
rm /usr/local/bin/mainuser
rm /usr/local/bin/newuser
rm /usr/local/bin/rmuser
rm /usr/local/bin/sharelink
```
