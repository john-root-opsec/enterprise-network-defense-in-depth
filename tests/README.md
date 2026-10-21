# 🧪 Network Connectivity and Security Tests

This directory documents the connectivity and security tests performed on the **Enterprise Network Defense-in-Depth** project in Cisco Packet Tracer.

## 📋 Test Plan

| Test | Expected Result | Evidence |
|---|---|---|
| Finance VLAN 20 → HR VLAN 30 | Ping succeeds, if permitted by the configured policies. | `screenshots/finance-to-hr.png` |
| Operations VLAN 60/70 → HR VLAN 30 | Ping is blocked by the applicable access policy. | `screenshots/operations-to-hr-blocked.png` |
| PC40 → TI laptops | Connectivity succeeds between the wired workstation and wireless clients. | `screenshots/ti-connectivity.png` |
| Internal application server | The internal portal or another configured service responds successfully. | `screenshots/internal-portal.png` |

## 🎯 Purpose

These tests help validate inter-VLAN routing, access control policies, wireless connectivity, and centralized network services.

> **Note:** Expected results must be confirmed through actual tests. Evidence should be added only after the corresponding behavior has been verified in Cisco Packet Tracer.
