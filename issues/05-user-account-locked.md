# Issue 05: User Account Locked

## Symptoms
- User cannot log in
- Error message: “The referenced account is currently locked out”
- Multiple failed login attempts

## Diagnostics
1. Confirm lockout with the user  
2. Check AD account status  
3. Verify lockout policy (threshold, reset time)

## Root Cause
Account locked due to multiple incorrect password attempts.

## Resolution
### Step 1 — Unlock from Active Directory
1. Open **Active Directory Users and Computers**
2. Search for the user
3. Right-click → *Unlock Account*
4. Reset password if needed

### Step 2 — Educate user
- Ensure user knows the correct password  
- Recommend using a password manager  

## Status
Resolved
