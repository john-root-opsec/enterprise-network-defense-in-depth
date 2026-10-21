# 📚 Technical Documentation

This directory contains the technical documentation for the **Enterprise Network Defense-in-Depth** project.

## 📂 Documentation Index

| File | Description |
|---|---|
| `network-architecture.md` | Network topology, devices, and overall architecture design. |
| `ip-addressing.md` | IPv4 addressing plan, subnets, and default gateways. |
| `vlan-design.md` | VLAN segmentation and departmental network organization. |
| `services.md` | DHCP, DNS, FTP, Web, email, and application services. |
| `dmz-firewall-acls.md` | DMZ isolation, ACL policies, and traffic filtering between network segments. |
| `aaa-radius.md` | Centralized administrative authentication using AAA/RADIUS. |
| `device-hardening.md` | SSHv2, Telnet deactivation, password protection, and login banners. |
| `nat-pat.md` | Network Address Translation, PAT overload, and simulated external connectivity. |

## 🎯 Purpose

This documentation describes the network architecture, addressing, services, and security mechanisms used in the corporate network simulation.

It supports technical analysis, troubleshooting, security validation, and future improvements to the infrastructure.

## 🔐 Security Scope

- **DMZ and ACLs:** Document isolation policies and traffic restrictions between internal networks and designated service segments.
- **AAA/RADIUS:** Document centralized authentication for administrative access to network devices.
- **Device Hardening:** Describe secure remote management, password protection, and access restrictions.
- **NAT/PAT:** Explain address translation and connectivity between the internal network and simulated external networks.

> **Note:** Security features should be described as implemented only after their configurations and behavior have been verified in Cisco Packet Tracer.
