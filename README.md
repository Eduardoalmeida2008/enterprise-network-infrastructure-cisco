# enterprise-network-infrastructure-cisco
"A complete multi-router enterprise network design featuring Inter-VLAN routing, OSPF dynamic routing, DHCP services, and advanced security through Extended Access Control Lists (ACLs) using Cisco Packet Tracer.

# Enterprise Network Infrastructure - Project 8.2

## 📌 Overview
This repository contains the complete documentation and configuration for **Project 8.2**. It features a complex multi-router topology designed to simulate a secure corporate environment using Cisco Packet Tracer. The project demonstrates advanced knowledge in Inter-VLAN routing, OSPF, and granular security policies.

## 🏗️ Technical Architecture
- **VLAN Management:** Full segmentation across 8 Switches (SW1-SW8).
- **Routing Protocol:** OSPF (Open Shortest Path First) ensuring full reachability between sites R1, R2, R3, and R4.
- **Dynamic Addressing:** Dedicated DHCP pools configured for each VLAN to automate host addressing.
- **Inter-VLAN Routing:** Router-on-a-Stick implementation using 802.1Q encapsulation.

## 🛡️ Security & Access Control (ACLs)
The project implements rigorous security via **Extended Access Control Lists (ACLs)**, specifically applied to protect sensitive zones.

### Security Logic Validated:
- **VLAN 50 Security:** Configured on **R2** to strictly allow traffic ONLY from **VLAN 60**. All other VLANs (including **VLAN 40**) are denied access to this segment.
- **VLAN 90 & 130 Protection:** Specific ACLs applied to these interfaces to ensure traffic isolation and authorized access only, as documented in the evidence files.
- **Edge Filtering:** Security is applied at the interface level, ensuring that filtering happens at the closest gateway point.

## 📁 Documentation Structure
The project is organized into 31 professional evidence files following a logical deployment sequence:

| Files | Description |
| :--- | :--- |
| **01 - 09** | Physical/Logical Topologies and Layer 2 Switch Setup (VLANs/Trunks). |
| **10 - 18** | Layer 3 Configurations: Interface Status, DHCP Pools, and OSPF Routing Tables. |
| **19 - 21** | **ACL Implementation:** Rules for VLAN 50, 90, and 130 security. |
| **22 - 25** | DHCP Client Success (IP acquisition evidence). |
| **26 - 31** | **Final Connectivity Tests:** Proving ACL effectiveness and inter-vlan communication. |

## 🛠️ Technologies Used
- Cisco IOS CLI
- OSPF Dynamic Routing
- Extended Access Control Lists (ACLs)
- IEEE 802.1Q Dot1Q
- DHCP Server Configuration

---
*Note: This project was developed as part of the 8.2 Infrastructure Lab, focusing on real-world security scenarios.*
