# Network Verification Result

Halaman ini mendokumentasikan **hasil verifikasi konektivitas, routing, dan kebijakan keamanan (ACL)** pada lab jaringan enterprise.

---

## 1️⃣ Verifikasi Routing

### OSPF & EIGRP Redistribution
- Route OSPF berhasil diterima di domain EIGRP sebagai **External Route (D EX)**
- Route EIGRP berhasil diterima di domain OSPF sebagai **External Route (O E2)**

**Command:**

![alt text](<Hands_On-Pratice-2/img/Show Eigrp.JPG>)

![alt text](<Hands_On-Pratice-2/img/Show OSPF.JPG>)

---
## 2️⃣ Verifikasi Access Control List (ACL)

### Kebijakan ACL
- VLAN 10 & VLAN 20 → HTTPS (TCP 443) ke `11.11.11.0/29` ✅
- VLAN 30, 40, 50, 60 → HTTPS ke `11.11.11.0/29` ❌
- Trafik selain HTTPS → diperbolehkan ✅

![alt text](<Hands_On-Pratice-2/img/Test ACL Web Server.JPG>)

---
### File Packet Tracer

[Hands_On Pratice 02](<Hands_On-Pratice-2/Hands_On Pratice 2.pkt>)
---