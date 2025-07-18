## X4Recon Project
![Python](https://img.shields.io/badge/Code-Python-blue?style=flat&logo=python&logoColor=white)
![Termux](https://img.shields.io/badge/Platform-Termux-brightgreen?style=flat&logo=android&logoColor=white)
![Kali Linux](https://img.shields.io/badge/Platform-Kali_Linux-black?style=flat&logo=kalilinux&logoColor=white)

## What is ***X4Recon*** specifically for Kali or Termux `(ROOT)`?
This tool functions to limit access to certain device connections on a local Wi-Fi network. The mechanism is carried out by scanning all devices connected to the local network via IP Gateway, then performing ARP Spoofing to trick the target device, and finally blocking the device's traffic with the help of firewall rules (iptables). This tool is useful for testing network security or education about MITM (Man-In-The-Middle) techniques and network traffic control.

![images](https://files.catbox.moe/1lhugo.png)

The screenshot above shows the display of the tools.

## Dependencies
- python3-pip
- net-tools 
- iproute2 
- iptables 
- tcpdump 
- libpcap-dev

## Installation
### Disclaimer: Use this tool in `Root` access.

1. Clonning Git Repository
```bash
git clone https://github.com/fkzsecxploit-id/X4Recon.git
```

2. Go to Project Repository
```bash
cd X4Recon
```

3. Install dependencies
```bash
pip3 install -r requirements.txt
```

4. Grant full access rights
```bash
chmod +x main.py
```

## Usage
To start the project Tools

```bash
python3.11 main.pyc
```

### Disclaimer: Use env to create a temporary environment.

## Available parameters
This case occurs when you have entered the tools

- `scan`: scans for online hosts on your network.
- `hosts`: show the hosts you have scanned.
- `arp`: To attack the ARP system for poisoning.

## Example reports

1. Hosts view
```sql
Index   IP Address      MAC Address             Hostname                Vendor
----------------------------------------------------------------------------------------------------
0       192.168.1.1     10:07:xx:xx:xx:xx       Unknown Fiberhome xxxxxxxxxx Technologies Co.,LTD
1       192.168.1.3     00:21:xx:xx:xx:xx       Unknown Intel Corporate
2       192.168.1.7     e0:41:xx:xx:xx:xx       Unknown zte corporation
3       192.168.1.2     60:dc:xx:xx:xx:xx       Unknown AltoBeam Inc.
4       192.168.1.5     c0:15:xx:xx:xx:xx       Unknown Unknown Vendor
5       192.168.1.4     d0:a4:xx:xx:xx:xx       Unknown China Dragon Technology Limited
6       192.168.1.8     b0:b5:xx:xx:xx:xx       Unknown GUANGDONG OPPO MOBILE TELECOMMUNICATIONS CORP.,LTD
7       192.168.1.9     1c:bf:xx:xx:xx:xx       Unknown Shenzhen Century Xinyang Technology Co., Ltd
```

2. Attack view
```sql
[+]  Starting ARP spoofing...

[+]  Target IP   : 192.168.1.5
[+]  Target MAC  : c0:15:xx:xx:xx:xx
[+]  Gateway MAC : 10:07:xx:xx:xx:xx

[+]  Block All Traffic for: 192.168.1.5
[!]  Starting ARP spoofing between 192.168.1.5 and gateway 192.168.1.1...
/usr/lib/python3/dist-packages/scapy/sendrecv.py:479: SyntaxWarning: 'iface' has no effect on L3 I/O send(). For multicast/link-local see https://scapy.readthedocs.io/en/latest/usage.html#multicast
  warnings.warn(
WARNING: You should be providing the Ethernet destination MAC address when sending an is-at ARP.
WARNING: You should be providing the Ethernet destination MAC address when sending an is-at ARP.
```

## 🔐 Security Feature 
- ARP Security / ARP Table Integrity
- Network Availability (DoS - Denial of Service)
- LAN Device Privacy
- Gateway Trust / Routing Integrity
- Service Exposure (Port 80 / HTTP status check)
- Host-based Firewall Bypass

## ⚠️ What are the risks involved?

This tool is intended **only for educational and authorized penetration testing purposes**. Unauthorized use is strictly prohibited and can result in legal consequences.

### ❗ Legal Risks
- Performing ARP spoofing or traffic blocking on public or unauthorized networks can **violate cybersecurity laws** (e.g., Indonesia’s UU ITE or international cybercrime laws).
- May be considered as **unauthorized access or denial-of-service (DoS)** attacks.

### ❗ Technical Risks
- Can disrupt the **internet connection of target devices**, making them unable to access the internet.
- May cause instability on the local network or overload the router.
- Could unintentionally **affect your own connection** if misconfigured.

### ❗ Detection Risks
- Activities such as ARP spoofing can be **detected by intrusion detection systems (IDS/IPS)**.
- Your device MAC address may be **blacklisted or banned** from the network.

### ❗ Ethical Considerations
- Unauthorized testing can breach **privacy, confidentiality, and trust**.
- Always obtain **explicit permission** before testing on any network that you do not own.

> 💡 This project is for learning and ethical hacking in controlled environments. Use responsibly.

## ⚠️ DISCLAIMER
X4Recon is designed for legal and ethical security testing.
- Use wisely
- Comply with applicable laws
- unauthorized use will be prosecuted by law

## Last Disclaimer
We are not responsible for your behavior, use it as wisely as possible.

## Thanks for :3
- null:Nothing_left.
- TC20
- Damnboy <3

## 📜 License
Distributed under the MIT License. See [MIT LICENSE](./LICENSE.txt) for more information.

## Links
[![YouTube Badge](https://img.shields.io/static/v1?label=|&message=YouTube&color=red&style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@fkzz_id?si=2iKh-_gak2JPjffW) [![Telegram Badge](https://img.shields.io/static/v1?label=|&message=Telegram&color=lightblue&style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/dlp46sec) [![Telegram Badge](https://img.shields.io/static/v1?label=|&message=Telegram2&color=lightblue&style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/noxleviathan404) [![TikTok Badge](https://img.shields.io/static/v1?label=|&message=TikTok&color=Gray&style=for-the-badge&logo=tiktok&logoColor=white)](https://tiktok.com/@fkzsec.id)
  
