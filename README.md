# Enterprise Network Lab (Cisco Packet Tracer)

Simulasi jaringan enterprise menggunakan **Cisco Packet Tracer** yang mengintegrasikan **OSPF, EIGRP, VLAN, dan Access Control List (ACL)**.

---

## Objective
- Mengimplementasikan routing dinamis **OSPF & EIGRP**
- Melakukan **route redistribution** antar routing protocol
- Menerapkan **VLAN & inter-VLAN routing**
- Mengontrol akses server menggunakan **Extended ACL**

---

## Network Summary
- **VLAN**: 10, 20, 30, 40, 50, 60  
- **Routing**:
  - OSPF (backbone)
  - EIGRP (distribution)
  - Redistribution pada ASBR  
- **Server Network**:
  - `11.11.11.0/29` (HTTPS restricted)
  - `44.44.44.0/29` (internal)

---

## Security Policy (ACL)
- ✅ VLAN 10 & VLAN 20 → HTTPS (TCP 443) ke `11.11.11.0/29`
- ❌ VLAN lain → HTTPS ke server
- ✅ Trafik selain HTTPS diperbolehkan
- ACL type: **Extended ACL**, applied **inbound on SVI**

---

## Key Takeaways
- Redistribution memungkinkan komunikasi antar domain routing
- VLAN meningkatkan segmentasi & manajemen jaringan
- ACL menerapkan prinsip **least privilege**
- Desain jaringan harus seimbang antara **routing dan security**


