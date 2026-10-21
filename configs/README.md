# ⚙️ Network Device Configurations

This directory documents the configuration and operational role of the network devices used in the **Enterprise Network Defense-in-Depth** project.

## 📂 Configuration Index

| File | Device | Description |
|---|---|---|
| `core-switch.txt` | Cisco 3560 | VLAN interfaces (SVIs), inter-VLAN routing, DHCP relay, and core connectivity. |
| `access-switches.txt` | Cisco 2960 | Access port assignments, VLAN configuration, and trunk links. |
| `edge-router.txt` | Cisco 2911 | Routing between the internal network and external networks, with NAT/PAT where configured. |
| `wireless-router.txt` | WRT300N | Wireless connectivity for TI laptops, wireless security, and LAN integration with PC40. |
| `security-configurations.txt` | Network devices | ACLs, SSHv2, AAA/RADIUS, password protection, and other security settings, where implemented. |

## 🏗️ Device Roles

- **Core Switch — Cisco 3560:** Performs Layer 3 switching and routes traffic between departmental VLANs.
- **Access Switches — Cisco 2960:** Connect end devices and provide access to the assigned VLANs.
- **Edge Router — Cisco 2911:** Connects the internal network to external networks when the required routing is configured.
- **Wireless Router — WRT300N:** Provides Wi-Fi connectivity to the TI laptops, supporting communication with the wired administrative workstation PC40 when correctly configured.

## 🎯 Purpose

This directory provides a structured reference for reviewing, documenting, troubleshooting, and reproducing device configurations in Cisco Packet Tracer.

Configuration files should contain verified commands, relevant interface settings, and concise explanations of each device's role.

## 🔐 Configuration and Security Scope

| Area | Configuration Details |
|---|---|
| **VLANs and Trunks** | VLAN creation, access ports, and permitted VLANs on trunk links. |
| **Inter-VLAN Routing** | SVIs, default gateways, and Layer 3 routing on the Cisco 3560. |
| **DHCP Relay** | Forwarding DHCP requests to the centralized server where required. |
| **Wireless Network** | WRT300N SSID, wireless security, LAN connectivity, and DHCP settings. |
| **Access Control** | ACL rules and traffic filtering between network segments. |
| **Secure Administration** | SSHv2, password protection, and AAA/RADIUS where configured. |
| **External Connectivity** | Static routing and NAT/PAT where implemented and tested. |

> **Note:** This index describes the configuration areas covered by the project. Only verified commands and tested features should be documented as implemented. Do not include real passwords, shared secrets, or other sensitive credentials.
