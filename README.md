# 🏢 Campus Area Network (CAN) - Packet Tracer Project

This project simulates a **Campus Area Network (CAN)** using Cisco Packet Tracer. The network spans **three buildings**, each containing devices logically segmented into **four VLANs**:

- `VLAN 10` - **ENG** (Engineering) — `10.0.0.0/24`
- `VLAN 20` - **SALES** — `192.168.20.0/24`
- `VLAN 30` - **HR** — `192.168.30.0/24`
- `VLAN 99` - **SERVER** — `192.168.99.0/24`

A **centralized DHCP server** in the SERVER VLAN (VLAN 99) handles IP address assignments for all VLANs across all three buildings.

Inter-VLAN routing is performed directly on a **Layer 3 switch** using SVIs (Switched Virtual Interfaces).

---

## 📁 File

- `Network.pkt` — Cisco Packet Tracer project file with full configuration.

---

## 📌 Features

- ✅ 802.1Q VLAN Trunking
- ✅ Layer 3 Switching for Inter-VLAN Routing (No Router-on-a-Stick)
- ✅ Central DHCP Server with Relay via `ip helper-address`
- ✅ Subnetting by Department
- ✅ Multi-building design with VLAN propagation

---

## ⚙️ Devices Used

- 1x **Layer 3 Switch** (for VLAN interfaces and routing)
- 3x **Access Switches** (1 per building)
- 1x **DHCP Server** (in VLAN 99)
- Multiple **end devices** in ENG, SALES, HR VLANs

---

## 📡 DHCP Configuration

- The DHCP server resides in **VLAN 99** (`192.168.99.0/24`)
- VLANs 10, 20, and 30 are configured with `ip helper-address` on the Layer 3 switch
- Each VLAN has its own DHCP pool configured on the server

---

## 🧪 Testing Instructions

1. Open `CAN_Network.pkt` in Cisco Packet Tracer.
2. Power on all devices.
3. Confirm that end devices in VLANs 10, 20, and 30 receive IP addresses from the DHCP server.
4. Ping across VLANs to confirm inter-VLAN routing.
5. Optionally test DNS or HTTP services if configured on the server.

---

## 👨‍💻 Author

**Blake Barth**  
📧 [blakebarth@proton.me](mailto:blakebarth@proton.me)  
🌐 [GitHub](https://github.com/Blake-Barth) | [LinkedIn](https://linkedin.com/in/Blake-Barth)
