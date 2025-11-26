# Issue 03: Slow Network Performance

## Symptoms
- Internet feels slow
- Applications loading slowly
- High latency during calls or VPN

## Diagnostics
1. Speed test to check actual bandwidth  
2. Check latency:

tracert google.com

3. Check running applications consuming bandwidth  
4. Verify Wi-Fi signal strength  
5. Check for packet loss using ping:

ping -n 20 8.8.8.8

## Root Cause
- Network congestion  
- Poor Wi-Fi signal  
- High latency from ISP  
- Background applications consuming bandwidth  

## Resolution
- Restart router if possible  
- Move device closer to access point  
- Disable large downloads  
- Contact ISP if latency > 200ms consistently  

## Status
Resolved
