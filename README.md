# 🖥️ Cybersecurity Homelab

## 📌 Overview
This repository documents my **cybersecurity-focused homelab** built on a **mini-PC** running **Proxmox**.  
The goal is to create a complete environment to:
- Host useful services (NAS, DNS filtering, firewall, etc...)
- Experiment with tools and network configurations
- Build a lab for security testing and attack analysis
- Practice on vulnerable machines

---

## 🗂️ Homelab Architecture

[Internet]
│
▼
[Mini-PC running Proxmox]
├── VM: TrueNAS (Network-attached storage)
├── LXC: Pi-hole (DNS filtering & ad blocking)
├── Future VM: pfSense (Firewall & routing)
    │
    ▼
    [ISP Router / Modem]
├── Various test VMs (services & servers)
└── Vulnerable machines for pentesting

---

## 🛠️ Current Components
- **Proxmox VE** – main hypervisor
- **TrueNAS** – centralized NAS storage
- **Pi-hole** – network-wide DNS filtering
- **Test VMs** – temporary machines for experimentation

---

## 📸 Screenshots

### Proxmox Dashboard
![Proxmox Dashboard](https://github.com/user-attachments/assets/32261b44-6a6b-4196-acb2-1c942e39ccd5)

### TrueNAS Storage View
![TrueNAS Storage](images/truenas_storage.png)

### Pi-hole Query Log
![Pi-hole Queries](images/pihole_queries.png)

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
| pfSense          | ⏳ Planned |
| Vulnerable VMs   | ⏳ Planned |
| Snort            | ⏳ Planned |

---

## 🔐 Security Notice
> ⚠️ Vulnerable environments are **isolated from the main network** and must never be directly exposed to the Internet.
