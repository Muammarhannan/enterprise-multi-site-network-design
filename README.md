# Enterprise Multi-Site Network Design

## 📖 Overview

This project demonstrates the design and implementation of a multi-site enterprise network using Cisco Packet Tracer.

The network consists of a Headquarters (HQ) site connected to Bandung and Jakarta branch offices through WAN links. The implementation focuses on VLAN segmentation, inter-VLAN routing, EtherChannel, static routing, and centralized network services.

---

## 🏢 Network Architecture

### Headquarters (HQ)

| VLAN | Department  | Network         | Gateway      |
| ---- | ----------- | --------------- | ------------ |
| 10   | Management  | 192.168.10.0/24 | 192.168.10.1 |
| 20   | IT          | 192.168.20.0/24 | 192.168.20.1 |
| 30   | HRD         | 192.168.30.0/24 | 192.168.30.1 |
| 40   | Finance     | 192.168.40.0/24 | 192.168.40.1 |
| 50   | Server Farm | 192.168.50.0/24 | 192.168.50.1 |

### Branch Offices

| Site    | Network          | Gateway       |
| ------- | ---------------- | ------------- |
| Bandung | 192.168.100.0/24 | 192.168.100.1 |
| Jakarta | 192.168.200.0/24 | 192.168.200.1 |

---

## 🌐 WAN Connectivity

| Link              | Network       |
| ----------------- | ------------- |
| HQ ↔ Bandung      | 10.10.10.0/30 |
| HQ ↔ Jakarta      | 10.10.20.0/30 |
| CORE1 ↔ HQ Router | 10.10.30.0/30 |

---

## 🔧 Technologies Used

### Routing & Switching

* VLAN Segmentation
* Inter-VLAN Routing
* 802.1Q Trunking
* Layer 3 Switching
* EtherChannel (LACP)

### WAN Connectivity

* Static Routing
* Multi-Site Network Design
* Point-to-Point WAN Links

### Network Services

* DHCP Server
* DNS Server
* WEB Server
* NTP Server
* SYSLOG Server

### Validation & Troubleshooting

* Inter-VLAN Testing
* WAN Connectivity Testing
* Branch-to-Branch Testing
* Service Accessibility Testing
* Network Troubleshooting

---

## 🧪 Validation Results

### Test 1 — Inter-VLAN Routing Validation

Verified communication between VLAN 20 (IT) and VLAN 30 (HRD) using Layer 3 switching on CORE1.

### Test 2 — Headquarters to Bandung Connectivity

Verified WAN connectivity between Headquarters and Bandung branch using static routing.

### Test 3 — Headquarters to Jakarta Connectivity

Verified WAN connectivity between Headquarters and Jakarta branch using static routing.

### Test 4 — Inter-Branch Communication

Validated communication between Bandung and Jakarta branch networks through centralized routing.

### Test 5 — Centralized Service Accessibility

Verified access from branch offices to services hosted in the HQ Server Farm VLAN.

---

## 🎯 Project Outcome

✅ Inter-VLAN Routing Operational

✅ HQ ↔ Bandung Connected

✅ HQ ↔ Jakarta Connected

✅ Bandung ↔ Jakarta Connected

✅ Centralized Services Accessible

---

## 📁 Project Files

* Packet Tracer topology (.pkt)
* Network topology diagram
* Validation screenshots
* Project documentation

---

## 👨‍💻 Author

Mu'ammar Hannan Najib

Aspiring Network Engineer | Cisco Networking | CCNA Learning Journey
