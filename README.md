# 🏫 Campus Network Design – Packet Tracer Project

## Overview

This repository contains the early layout and planning files for a multi-site campus network simulation in Cisco Packet Tracer. The goal of this project is to build a realistic, modular, and redundant network topology that allows for hands-on practice with a wide range of networking technologies.

> **Status:** 🚧 *In early layout and planning phase*

---

## 📐 Network Design Highlights

This design follows a **3-tier hierarchical model** deployed across **two campus locations**, each with redundant routing and switching:

- **Core Layer:**
  - 2 redundant Cisco 4331 routers
  - 2 Layer 3 switches (Cisco 3560) per site
- **Distribution Layer:**
  - 4 Layer 2 switches (per site)
- **Access Layer:**
  - 4 Layer 2 switches (per site)
- **Inter-site connection:** Planned via WAN link (e.g. simulated serial, fiber, or VPN)

---

## 🛠️ Configuration Goals

This network will be used to practice the configuration and integration of:

- ✅ **VLANs** (segmentation by department, building, etc.)
- ✅ **Inter-VLAN routing** (via Layer 3 switches or routers)
- ✅ **DHCP** (central or distributed address assignment)
- ✅ **DNS** (internal name resolution)
- ✅ **LAN/WAN topologies** (multi-site communication and routing)
- ✅ **IP Phones and Voice VLANs** (VoIP network simulation)
- ✅ **Redundant links** (STP, EtherChannel)
- ✅ **Dynamic Routing Protocols** (OSPF, EIGRP)
- ✅ **Security policies** (basic ACLs and port security)
- ✅ **NTP, SNMP, and Syslog** (optional network services for monitoring)

---

## 🔧 Tools Used

- **Cisco Packet Tracer 8.x**
- Standard Cisco routers and switches:
  - Cisco 4331 ISR (core routers)
  - Cisco 3560 (Layer 3 switches)
  - Cisco 2960 (Layer 2 switches)
- Simulated end devices:
  - PCs
  - IP Phones
  - Printers
  - Servers (DHCP, DNS, etc.)

---

## 🧪 Planned Use Cases

- Hands-on practice for CCNA-level topics
- Campus LAN and WAN simulation
- VLAN and IP addressing schema design
- High availability (redundant core/distribution layers)
- Testing network scalability and service integration

---

## 🚀 Future Enhancements

- Add server services: FTP, web, email
- Configure failover gateway protocols (HSRP/VRRP)
- Introduce network monitoring and logging tools
- Simulate security policies (ACLs, DMZ, switchport security)

---

## 📁 Files

- `campus_network_v0.pkt` – Initial topology layout (in progress)
- `topology_diagram.png` – Visual map of the network (coming soon)
- `config_snippets/` – Saved configuration templates and commands (coming soon)

---

## 👨‍💻 Author

**Blake Barth**  
Security-focused tech enthusiast | CompTIA Security+ | Studying for CCNA  
Passionate about network automation, Linux internals, and practical lab simulations.
