# 🧪 Network Connectivity and Security Tests

This directory documents the connectivity and security tests performed on the **Enterprise Network Defense-in-Depth** project in Cisco Packet Tracer.

## 📋 Test Plan

| Test | Expected Result | Evidence |
|---|---|---|
| Finance VLAN 20 → HR VLAN 30 | Ping succeeds when permitted by the configured policies. | `screenshots/finance-to-hr.png` |
| Operations VLAN 60/70 → HR VLAN 30 | Ping is blocked by the applicable access control policy. | `screenshots/operations-to-hr-blocked.png` |
| PC40 → TI laptops | Connectivity succeeds between the wired workstation and wireless clients. | `screenshots/ti-connectivity.png` |
| Internal application server | The internal portal or another configured service responds successfully. | `screenshots/internal-portal.png` |

## 🎯 Purpose

These tests validate inter-VLAN routing, access control policies, wireless connectivity, and centralized network services.

> **Note:** Expected results must be confirmed through actual tests. Evidence should be added only after the corresponding behavior has been verified in Cisco Packet Tracer.

---

## ✅ Test Evidence: Finance to HR Connectivity

**Test ID:** `NET-TEST-01`

**Source:** PC20 — Finance, VLAN 20  
**Source IP:** `192.168.20.11`  
**Destination:** PC31 — HR, VLAN 30  
**Destination IP:** `192.168.30.12`

**Command:**

```text
ping 192.168.30.12
```

**Result:** Successful — 4 packets received, 0% packet loss on the final attempt.

**Conclusion:** Inter-VLAN connectivity between Finance and HR was successfully verified in Cisco Packet Tracer.

### Screenshot

![Finance to HR connectivity test](screenshots/finance-to-hr.png)

---

## 🔒 Remaining Tests

The following evidence will be added after each test has been executed and verified:

- **NET-TEST-02:** Confirm that traffic from Operations VLAN 60 or 70 to HR VLAN 30 is blocked by the configured ACL.
- **NET-TEST-03:** Verify communication between PC40 and the TI laptops over the wireless network.
- **NET-TEST-04:** Access the internal application portal and confirm that the service responds successfully.
