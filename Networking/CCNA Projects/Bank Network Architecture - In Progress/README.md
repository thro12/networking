# Bank Network Architecture and Configuration (In Progress)

**Status:** In progress (started November 2026) - not yet verified end to end.

Four-floor, twelve-department bank network simulation in Cisco Packet Tracer, built following the concept and requirements of a public bank network case study.

## Topology and design
- PCs, printers and wireless access points in each department for Wi-Fi client access
- Per-department VLAN segmentation
- Routed connectivity between floors
- OSPF routing and centralized DHCP services
- Topology and configuration are built with Packet Tracer's PTBuilder script module (JavaScript)

## Files
- [bank-build-only-v9.js](https://github.com/thro12/networking/blob/main/Networking/CCNA%20Labs/Bank%20Network%20Architecture%20-%20In%20Progress/bank-build-only-v9.js) - run in an empty Packet Tracer project: places all devices, modules and cables
- [bank-config-only-v10.js](https://github.com/thro12/networking/blob/main/Networking/CCNA%20Labs/Bank%20Network%20Architecture%20-%20In%20Progress/bank-config-only-v10.js) - run once after the build: applies interface, VLAN, DHCP, OSPF and service configuration

## Verified so far (10 Nov 2026)
Build completes with no failed calls; 37 service-configuration checks OK; floor-1 interfaces up/up; 5 OSPF neighbours FULL.

## Still in progress
End-to-end connectivity checks, DHCP for five endpoints currently receiving link-local addresses, and remaining security and mail service configuration.
