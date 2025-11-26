# Network Troubleshooting Guide

This repository contains real-world network issues and step-by-step troubleshooting procedures for IT Support and Technical Support roles.

---

##  1. No Internet – DNS Issue

### Symptoms:
- Connected to Wi-Fi/Ethernet but no internet access.
- Websites not loading.

### Troubleshooting Steps:
1. Test basic connectivity:
ping 8.8.8.8

2. Test DNS resolution:

ping google.com

3. Check DNS settings:

ipconfig /all

4. Use NSLOOKUP:

nslookup google.com

### Cause:
- Incorrect DNS or DNS server not responding.

### Solution:

ipconfig /flushdns netsh int ip set dns "Wi-Fi" static 8.8.8.8

---

##  2. Printer Offline

### Symptoms:
- Printer shows “Offline”
- Documents stuck in queue

### Troubleshooting:
1. Check cable or Wi-Fi connection.
2. Restart Print Spooler:

net stop spooler net start spooler

3. Clear print queue if needed.

---

##  3. Slow Network Performance

### Troubleshooting:
- Check speed test results.
- Use TRACERT to diagnose latency:

tracert google.com

- Check for high-bandwidth applications.

---

##  4. IP Conflict

### Troubleshooting:
- Identify conflict:

arp -a

- Renew IP:

ipconfig /release ipconfig /renew

---

##  5. User Account Locked

### Troubleshooting:
- Reset user from Active Directory.
- Verify security policies (account lockout threshold).

---

✔ More troubleshooting scenarios coming soon.
