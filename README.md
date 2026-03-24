# Help Desk Lab – AD & Domain Setup

## Lab Setup: VirtualBox Client and Server
- Server and client VMs configured on an internal network.
![Client Setup](client-about.png)
![Server Setup](server-about.png)

## Active Directory
- Set up an Active Directory domain
- Configured client IP and DNS settings to ensure connectivity
![Client Setup](local%20server%20info.png)
![Client Setup](client-domain.png)
- Tested connectivity using ipconfig /all
![Client Setup](client%20ipconfig%20-%20ping%20+%20nslookup%20results.png)

- Created Organizational Units
![Client Setup](AD%20OU's.png)

## Security Groups & Network Shares
- Created security groups in AD to manage access to department-specific network shares  
- Set folder permissions accordingly
![Client Setup](HR_Share%20group.png)
![Client Setup](HR_Share%20Permissions.png)
![Client Setup](client%20access%20hr%20share.png)

## Policies
- Set account lockout and password policies for users and used gpupdate /force to apply
- Simulated an account unlock and password reset
![Client Setup](account%20lockout%20policy.png)
![Client Setup](password%20policy.png)
![Client Setup](unlock%20account%20+%20reset%20user%20password.png)
