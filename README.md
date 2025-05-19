# Networking-Simulator-Ex-Comapany
# Advanced Networking Simulation with Cisco Packet Tracer

This project is a comprehensive networking simulation built using Cisco Packet Tracer. It demonstrates a multi-autonomous system topology that integrates dynamic and static routing protocols, NAT configurations, DHCP services, cloud connectivity, and access control policies.

## 🧠 Project Overview

The network topology simulates an enterprise-scale infrastructure with the following major components:

- Multiple Autonomous Systems (AS) connected via Border Gateway Protocol (BGP)
- Use of OSPF (Open Shortest Path First), EIGRP (Enhanced Interior Gateway Routing Protocol), and static routing
- Integration of Hybrid Fiber-Coaxial (HFC) and Digital Subscriber Line (DSL) clouds
- Network Address Translation (NAT):
  - Dynamic NAT on HFC-Home and DSL-Home routers
  - Static NAT on R7 for web servers
- Dynamic Host Configuration Protocol (DHCP) for automated IP assignment
- Access Control Lists (ACLs) for security and traffic restriction
- Redistribution of internal routing protocols into BGP for global reachability

## 🌐 Topology Highlights

- 🔴 **Red Circles**: Internal LANs using private IP addresses and static routing
- 🔵 **Blue Circles**: Home networks utilizing Dynamic NAT and DHCP
- 🟡 **Yellow Circles**: Web servers behind Static NAT, accessible publicly

## ✅ Features Implemented

1. **Hostnames Configured** on all routers
2. **IP Addressing** for all interfaces and end devices, except DHCP-enabled clients (PCs D, E, F, G)
3. **DHCP Server and Client Setup** on routers HFC-Home and DSL-Home
4. **Dynamic NAT** on routers HFC-Home and DSL-Home
5. **Static NAT** on router R7 for the networks 10.0.1.0/24 and 10.0.2.0/24
6. **Routing Configurations**:
   - AS 2500: OSPF with route propagation
   - AS 2700: Static routing
   - AS 2100: EIGRP with static default routes
   - AS 2200: OSPF with propagation
7. **BGP Configuration** between ASes
8. **IGP Redistribution into BGP**
9. **ACL Rules**:
   - Deny Telnet access to router HFC-Network from outside the HFC network
   - Block HTTP traffic from the 33.0.0.0/24 network, but allow all other services

## 🧪 Lessons Learned

- Route redistribution between interior and exterior gateway protocols must be precise to avoid loops and blackholes.
- NAT and ACL configurations can significantly impact reachability and security.
- DHCP automation helps reduce manual configuration errors.
- Debugging connectivity in multi-AS setups improves real-world troubleshooting skills.


## 👨‍💻 Author

**Shivain Maini**  
Cybersecurity & Networking Enthusiast  

---

