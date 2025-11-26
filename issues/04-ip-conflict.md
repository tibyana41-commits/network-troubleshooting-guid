# Issue 04: IP Address Conflict

## Symptoms
- Windows message: “IP address conflict detected”
- Device disconnects from the network
- Intermittent connectivity issues

## Diagnostics
1. Display ARP table:

arp -a

2. Check assigned IP address:

ipconfig

3. Verify if another device is using the same IP  
4. Check DHCP server for duplicate leases  

## Root Cause
Two devices on the same network are using the same static IP address or DHCP assigned duplicate IP.

## Resolution
### Option 1 — Renew IP:

ipconfig /release ipconfig /renew

### Option 2 — Assign manual IP  
For static IP environments, assign new IP outside conflict range.

### Option 3 — Fix DHCP scope  
Ensure IP range and reservations do not overlap.

## Status
Resolved
