# 🖥️ Cybersecurity Homelab

## 📌 Overview
This repository documents my **cybersecurity-focused homelab** built on a **mini-PC** running **Proxmox**.  
The goal is to create a complete environment to:
- Host useful services (NAS, DNS filtering, cloud storage, firewall, etc...)
- Experiment with tools and network configurations
- Build a lab for security testing and attack analysis
- Practice on vulnerable machines
- **Access the entire lab securely from anywhere via Tailscale VPN**

---

## 🗂️ Homelab Architecture
```
[Internet]
│
▼
[Mini-PC running Proxmox]
├── VM: TrueNAS (Network-attached storage)
├── VM: pfSense (Firewall & routing)
├── LXC: Pi-hole (DNS filtering & ad blocking)
├── VM: Nextcloud (Personal cloud for files & course material)
    │
    ▼
    [ISP Router / Modem]
├── Various test VMs (services & servers)
└── Vulnerable machines for pentesting
```
---

## 🛠️ Current Components
- **Proxmox VE** – main hypervisor
- **TrueNAS** – centralized NAS storage
- **Pi-hole** – network-wide DNS filtering
- **Nextcloud** – personal cloud storage for courses and files
- **Test VMs** – temporary machines for experimentation
- **Tailscale** – VPN connectivity to access all services securely from anywhere

---

## 📸 Screenshots

### Proxmox Dashboard
![Proxmox Dashboard](https://github.com/user-attachments/assets/32261b44-6a6b-4196-acb2-1c942e39ccd5)

### TrueNAS Storage View
![TrueNAS Storage](https://github.com/user-attachments/assets/a35ada8b-2d23-447f-8e60-b4a91a51d9df)
![TrueNAS Storage on Windows](https://github.com/user-attachments/assets/9d580904-9bc1-4825-9a57-f83d61a2bf74)

### Pi-hole Query Log
![Pi-hole Querie](https://github.com/user-attachments/assets/5e5b45c4-ca90-471e-8661-a3f176094411)

### Tailscale Dashboard
![Tailscale Dashboard](https://github.com/user-attachments/assets/53bbd998-3e02-40b2-9078-6cbe6c570b04)

---

## 🛡️ Pi-hole Blocklists

Here are the blocklists currently configured on my Pi-hole for enhanced ad and tracker blocking:

- [StevenBlack’s Unified Hosts](https://github.com/StevenBlack/hosts)
- [Mullvad Blocklists](https://github.com/mullvad/dns-blocklists?tab=readme-ov-file#lists)

---

## 📌 Resources & References
- [Proxmox Documentation](https://pve.proxmox.com/wiki/Main_Page)
- [TrueNAS Docs](https://www.truenas.com/docs/)
- [Pi-hole Documentation](https://docs.pi-hole.net/)
- [pfSense Docs](https://docs.netgate.com/pfsense/en/latest/)

---

## 📝 Progress Status
| Service          | Status     |
|------------------|-----------|
| Proxmox          | ✅ Installed |
| TrueNAS          | ✅ Installed |
| Pi-hole          | ✅ Installed |
| Nextcloud        | ✅ Installed |
| pfSense          | ✅ Installed |
| Tailscale VPN    | ✅ Installed & configured |
| Vulnerable VMs   | ⏳ Planned |
| Snort            | ⏳ Planned |

---
