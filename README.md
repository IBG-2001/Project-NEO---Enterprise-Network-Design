## Project Overview

Proyecto NEO is an enterprise network design project based on a multi-branch architecture.

The network consists of four branches interconnected through a WAN/cloud.  
Each branch contains six offices, and each office is composed of three main departments.

The design focuses on scalability, logical segmentation and enterprise best practices, including:
- VLAN-based segmentation per department
- Centralized DHCP per branch
- Inter-VLAN routing using Router-on-a-Stick
- Dynamic routing with OSPF
- Hierarchical IP addressing for future growth

# Changelog

All notable changes to this project will be documented in this file.

---

## [Unreleased]
- Security hardening (ACLs, Port Security, DHCP Snooping)
- STP root bridge tuning
- Documentation improvements

---

## [v1.0] – Initial Architecture
- Defined overall enterprise network topology
- Designed a four-branch architecture interconnected through a WAN/cloud
- Established branch structure with offices and departments
- Implemented VLAN-based segmentation per department
- Configured Inter-VLAN routing using Router-on-a-Stick
- Implemented centralized DHCP per branch

---

## [v2.0] – Hierarchical IP Addressing
- Redesigned IP addressing scheme using hierarchical allocation
- Assigned a /16 network per branch for scalability
- Implemented /24 subnets per VLAN
- Eliminated overlapping subnets
- Improved route summarization capabilities

---

## [v3.0] – OSPF Multi-Area Design
- Refactored OSPF configuration into a multi-area design
- Reserved Area 0 for core/WAN connectivity
- Assigned separate OSPF areas per branch
- Improved routing scalability and convergence
