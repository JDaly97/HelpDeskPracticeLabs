# Help Desk Lab – AD & Domain Setup

## Lab Setup: VirtualBox Client and Server
### Environment:
- Windows Server 2022 (Domain Controller)
- Windows 10 Client
- Active Directory Domain Services (AD DS)
- Virtualisation software (VirtualBox)
- Server and client VMs configured on the same internal network.
![Client Setup](screenshots/client-about.png)
![Server Setup](screenshots/server-about.png)

## Active Directory
- Set up an Active Directory domain
- Configured client IP and DNS settings to ensure connectivity
![Client Setup](screenshots/local%20server%20info.png)
![Client Setup](screenshots/client-domain.png)
- Tested connectivity using ipconfig /all
![Client Setup](screenshots/client-ipconfig-results.png)

- Created Organizational Units
![Client Setup](screenshots/AD%20OU's.png)

## Security Groups & Network Shares
- Created security groups in AD to manage access to department-specific network shares  
- Set folder permissions accordingly
![Client Setup](screenshots/HR_Share%20group.png)
![Client Setup](screenshots/HR_Share%20Permissions.png)
![Client Setup](screenshots/client%20access%20hr%20share.png)

## Policies
- Set account lockout and password policies for users and used gpupdate /force to apply
- Simulated an account unlock and password reset
![Client Setup](screenshots/account%20lockout%20policy.png)
![Client Setup](screenshots/password%20policy.png)
![Client Setup](screenshots/unlock%20account%20+%20reset%20user%20password.png)
