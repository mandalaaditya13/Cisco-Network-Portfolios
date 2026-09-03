# Enterprise Network Design & Implementation (CCNA Portfolio)

An enterprise-scale network infrastructure design and configuration project created during professional networking training and CCNA bootcamp, focused on high availability, security, and scalable routing.

## 📌 Project Overview
This project simulates a multi-department enterprise network capable of supporting 600+ staff across multiple core floors/locations. It implements a hierarchical network design model (Access, Distribution, and Core layers) to ensure optimal traffic flow, fault tolerance, and secure segmentation between departments (HR, Finance, Management, and IT).

## ⚙️ Core Architecture & Network Design
1. **Hierarchical Design:** Implements a structured 3-layer architecture (Core, Distribution, Access) utilizing Cisco Catalyst switches and routers to minimize broadcast domains and isolate network failures.
2. **Dynamic Routing (OSPF):** Configured Open Shortest Path First (OSPF) Single Area/Multi-Area across routers to establish automated path selection and seamless routing convergence.
3. **Gateway Redundancy (HSRP):** Implemented Hot Standby Router Protocol (HSRP) on distribution switches/routers to provide automatic gateway failover and zero downtime for end-users.
4. **VLAN & Trunking:** Logical network segmentation using 802.1Q trunking, native VLAN security, and Inter-VLAN routing via Router-on-a-Stick or Layer 3 switching.
5. **Security & Perimeter:** Applied Access Control Lists (ACLs) to restrict inter-departmental traffic (e.g., preventing HR from accessing Finance servers) and secured switch ports using Port-Security.
6. **NAT & DHCP Services:** Configured NAT Overload (PAT) for reliable public internet access sharing and set up automated DHCP server scopes with helper addresses (`ip helper-address`).

## 🛠️ Technology & Protocol Stack
* **Routing Protocols:** OSPF, Static Routing, Default Routing
* **Redundancy Protocols:** HSRP (Hot Standby Router Protocol)
* **LAN Technologies:** VLANs, 802.1Q Trunking, EtherChannel (Port Aggregation), STP (Spanning Tree Protocol)
* **Security & Services:** Standard/Extended ACLs, Port-Security, NAT (PAT), DHCP Server
* **Simulation Tools:** Cisco Packet Tracer, GSN3 / EVE-NG (Compatible)

## 📂 Repository Structure
* `/topology` : Contains the Cisco Packet Tracer topology file (`.pkt`) and exported topology layout images.
* `/configurations` : Contains text-based device configuration scripts (`.txt` or `.rsc`) for Cisco Routers, Switches, and MikroTik gateways.

## 🖼️ Network Topology
* **Top-Level Enterprise Topology:** ![Network Topology](Network%20Topologi.png)
