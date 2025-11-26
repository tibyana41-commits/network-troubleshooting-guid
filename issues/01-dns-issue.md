# Issue 01: No Internet – DNS Issue

## Symptoms
- Connected to Wi-Fi/Ethernet but no internet.
- Websites not loading.
- DNS resolution failing.

## Diagnostics

ping 8.8.8.8
ping google.com
ipconfig /all
nslookup google.com

## Root Cause
DNS server not responding or incorrect DNS configuration.

## Resolution

ipconfig /flushdns
netsh int ip set dns "Wi-Fi" static 8.8.8.8

## Status
Resolved
