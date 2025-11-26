# Issue 02: Printer Offline

## Symptoms
- Printer status shows “Offline”
- Documents stuck in the print queue
- Users unable to print

## Diagnostics
1. Check if printer is powered on  
2. Check network or USB connection  
3. Verify printer IP address  
4. Restart Print Spooler:

net stop spooler
net start spooler

## Root Cause
Print Spooler service stopped or communication issue between PC and printer.

## Resolution
- Restart Print Spooler
- Clear print queue if needed
- Reinstall printer driver
- Ensure correct network connectivity

## Status
Resolved
