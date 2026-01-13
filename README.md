# enterprise-network-infrastructure-cisco
"A complete multi-router enterprise network design featuring Inter-VLAN routing, OSPF dynamic routing, DHCP services, and advanced security through Extended Access Control Lists (ACLs) using Cisco Packet Tracer.

## 📌 Overview
This project demonstrates the design and implementation of a scalable enterprise network architecture. It focuses on core networking concepts including Layer 2 switching, Layer 3 routing, and perimeter security. The entire environment was simulated and validated using **Cisco Packet Tracer**.

## 🏗️ Architecture Features
- **VLAN Segmentation:** Organized departmental traffic across 8 managed switches.
- **Inter-VLAN Routing:** Implemented via Router-on-a-Stick (Dot1Q encapsulation).
- **Dynamic Routing:** OSPF protocol for seamless communication between four distinct router sites (R1-R4).
- **Core Services:** Automated IP addressing via DHCP pools configured on edge routers.
- **Security & Access Control:** - Implementation of **Extended Access Control Lists (ACLs)**.
  - Granular traffic filtering (e.g., restricted access to VLAN 50, allowing only VLAN 60).
  - Perimeter protection for sensitive network zones (VLAN 90 and 130).

## 📁 Project Structure & Documentation
The project is documented with 31 high-resolution evidence files, organized for easy auditing:

| Phase | Content |
| :--- | :--- |
| **01-09** | Physical/Logical Topologies and Layer 2 Switch Configurations |
| **10-18** | Layer 3 Routing (OSPF), Interface Status, and Global Routing Tables |
| **19-21** | Security Policies (Extended ACL Configuration) |
| **22-25** | DHCP Client Validations |
| **26-31** | Connectivity Testing (Ping tests proving successful routing and active ACL blocks) |

## 🛡️ Security Logic (ACL Validation)
The network follows the **Principle of Least Privilege**. 
- **Target:** VLAN 50 (Secure Zone).
- **Policy:** Only VLAN 60 (Authorized) can access VLAN 50. 
- **Validation:** Pings from VLAN 40 to VLAN 50 result in `Destination Host Unreachable`, confirming the ACL is correctly applied to the interface gateway.



## 🚀 How to Run
1. Download the `.pkt` file from the repository.
2. Open it in **Cisco Packet Tracer (v8.2 or higher)**.
3. Run the "Simulation Mode" to observe packet filtering in real-time at Router R2.

## 🛠️ Technologies Used
- Cisco IOS (Command Line Interface)
- OSPF (Open Shortest Path First)
- IEEE 802.1Q (VLAN Tagging)
- Extended ACLs (Access Control Lists)
- DHCP (Dynamic Host Configuration Protocol)
