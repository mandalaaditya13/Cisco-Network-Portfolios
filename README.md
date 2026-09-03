# Enterprise Network Design & Implementation (CCNA Portfolio)

An enterprise-scale network infrastructure design and configuration project created during professional networking training and CCNA bootcamp, focused on high availability, secure routing, and automated network services.

## 📌 Project Overview
This project simulates a multi-department enterprise network capable of supporting 600+ staff across multiple core locations. It implements a hierarchical network design model (Access, Distribution, and Core layers) to ensure optimal traffic flow, fault tolerance, and secure segmentation between departments (HR, Finance, Management, and IT).

## ⚙️ Core Architecture & Network Design
1. **Hierarchical Design:** Implements a structured 3-layer architecture (Core, Distribution, Access) utilizing Cisco Catalyst switches and routers to minimize broadcast domains and isolate network failures.
2. **Dynamic Routing (OSPF):** Configured Open Shortest Path First (OSPF) Single Area/Multi-Area across routers and multilayer switches to establish automated path selection and seamless routing convergence.
3. **Gateway Redundancy (HSRP):** Implemented Hot Standby Router Protocol (HSRP) on distribution switches/routers to provide automatic gateway failover and zero downtime for end-users.
4. **VLAN & Inter-VLAN Routing:** Logical network segmentation using 802.1Q trunking and SVI (Switched Virtual Interfaces) on Multilayer Switches to route traffic between different departments.
5. **Security & Filtering (ACL):** Applied Extended ACLs to restrict specific traffic (such as blocking unauthorized web/social media access) and secured switch ports using Port-Security.
6. **NAT Overload (PAT) & DHCP:** Configured **Standard ACLs** to identify and permit private internal IP subnets to be translated into public IP addresses via NAT Overload (PAT), alongside automated DHCP server scopes utilizing `ip helper-address`.

## 🛠️ Technology & Protocol Stack
* **Routing Protocols:** OSPF, Static Routing, Default Routing
* **Redundancy Protocols:** HSRP (Hot Standby Router Protocol)
* **LAN Technologies:** VLANs, 802.1Q Trunking, SVI, STP (Spanning Tree Protocol)
* **Security & Services:** Standard/Extended ACLs, Port-Security, NAT Overload (PAT), DHCP Server & IP Helper
* **Simulation Tools:** Cisco Packet Tracer

## 📂 Repository Structure
* Root files contain the Cisco Packet Tracer topology simulation (`.pkt`), topology layout image, and the comprehensive CLI command reference (`cli-reference.txt`).

## 🖼️ Network Topology
* **Top-Level Enterprise Topology:** ![Network Topology](Network%20Topologi.png)
