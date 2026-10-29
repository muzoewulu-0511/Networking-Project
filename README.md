# Departmental Network Design and Configuration – Cisco Packet Tracer

![Networking](https://img.shields.io/badge/Project-Networking-blue)
![Cisco Packet Tracer](https://img.shields.io/badge/Tool-Cisco%20Packet%20Tracer-informational)
![Status](https://img.shields.io/badge/Status-Academic%20Project-green)

## Project Overview

This project demonstrates the design and configuration of a basic departmental computer network using Cisco Packet Tracer.

The network consists of three departments: Administration, Sales, and Human Resources (HR). Each department has a dedicated switch connected to a central router, with two PCs assigned to each department. A server is also connected to the Administration department.

The project explores IP addressing, router configuration, network connectivity testing, and the use of Access Control Lists (ACLs) to restrict communication between selected departmental networks.

## Problem Statement

Organizations often need to connect multiple departments while maintaining appropriate communication restrictions between them.

This project demonstrates how a small departmental network can be structured to support communication between selected devices while applying network-level access restrictions to control traffic between departments.

## Project Objectives

- Design a departmental network topology.
- Connect three departmental switches to a central router.
- Connect two PCs to each departmental switch.
- Connect a server to the Administration department.
- Configure IP addressing for departmental devices.
- Test network connectivity using the ping command.
- Verify communication between selected departmental devices.
- Implement an Access Control List (ACL) to restrict communication between HR and Administration devices.

## Network Topology

The network contains the following components:

| Department / Component | Network Role | Devices |
|-------------------------|--------------|---------|
| Administration | Departmental network | Switch and 2 PCs |
| Sales | Departmental network | Switch and 2 PCs |
| Human Resources | Departmental network | Switch and 2 PCs |
| Router | Central network device | 1 router |
| Server | Connected to Administration | 1 server |

### Topology Design

The router is intended to connect the three departmental switches:

- Administration switch
- Sales switch
- HR switch

Each departmental switch connects two PCs. The server is connected to the Administration department.

**Note:** The submitted topology screenshot shows red connection indicators between the router and departmental switches. These links should be verified before describing the topology as fully operational.

## IP Address Configuration

The assignment documents the following IP addresses for one PC in each department:

| Department | Device | IP Address |
|------------|--------|------------|
| Administration | PC1 | `192.198.10.10` |
| Sales | PC1 | `192.198.20.11` |
| Human Resources | PC1 | `192.198.30.10` |

The screenshots also show successful DHCP requests.

The DHCP server configuration, subnet masks, default gateways, and complete IP addressing plan were not documented in the submitted report.

## Key Features and Activities

### 1. Network Topology Design

Created a departmental network topology in Cisco Packet Tracer with:

- One central router.
- Three departmental switches.
- Two PCs per department.
- One server connected to Administration.

### 2. IP Address Configuration

Configured and documented IP addresses for representative PCs in the Administration, Sales, and HR departments.

### 3. Network Connectivity Testing

Used ping tests to evaluate communication between devices in different departments.

The assignment documents a successful ping from a Sales PC to an Administration PC. Although the initial request timed out, the subsequent ping showed zero packet loss.

### 4. Access Control List Configuration

Configured an ACL through the router command-line interface to deny network access between HR and Administration devices.

The assignment demonstrates this restriction through an unsuccessful ping test from an HR PC to an Administration PC.

### 5. Router CLI Configuration

Used the router command-line interface to configure network interfaces and apply the access restriction.

The submitted report references the router configuration but does not provide the complete command sequence.

## Technologies and Tools Used

| Technology / Tool | Purpose |
|-------------------|---------|
| Cisco Packet Tracer | Network topology design and simulation |
| Router CLI | Router interface and ACL configuration |
| IP Addressing | Identification and communication of network devices |
| DHCP | IP configuration process demonstrated in the assignment |
| Ping | Network connectivity testing |
| Access Control Lists (ACLs) | Restricting communication between selected networks |

## Project Screenshots

The original assignment contains five screenshots documenting the project:

| Screenshot | Description |
|------------|-------------|
| Screenshot 1 | Completed departmental network topology |
| Screenshot 2 | IP address configuration on departmental PCs |
| Screenshot 3 | Successful ping from Sales to Administration |
| Screenshot 4 | Failed ping from HR to Administration |
| Screenshot 5 | ACL command configured through the router CLI |

Add the screenshots to the repository and update the paths below.

```text
screenshots/
├── network-topology.png
├── ip-configuration.png
├── successful-ping-sales-admin.png
├── failed-ping-hr-admin.png
└── acl-configuration.png
