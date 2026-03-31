# Help Desk Lab – AD & Domain Setup

## Lab Setup: VirtualBox Client and Server
### Environment:
- Windows Server 2022 (Domain Controller)
- Windows 10 Client
- Active Directory Domain Services (AD DS)
- Virtualisation software (VirtualBox)

Server and client VMs configured on the same internal network.
![Client Setup](screenshots/client-about.png)
![Server Setup](screenshots/server-about.png)

## Active Directory
Set up an Active Directory domain (JoshLab.local)
  
![Client Setup](screenshots/AD-domain.png)

![Client Setup](screenshots/local%20server%20info.png)

Ensured client connectivity and used ping + nslookup to confirm
![Client Setup](screenshots/client-domain.png)

![Client Setup](screenshots/client-ping-nslookup.png)

## Organisational Units, Security Groups & Network Shares

- Created Organisational Units to logically organise users and resources within the domain.
![Client Setup](screenshots/AD%20OU's.png)

- Created security groups to manage access to department-specific network shares
![Client Setup](screenshots/HR_Share%20group.png)

- Set folder permissions accordingly
![Client Setup](screenshots/HR_Share%20Permissions.png)

- Accessed the HR department network share from the client machine
![Client Setup](screenshots/client%20access%20hr%20share.png)

## Policies and Restrictions
- Set account lockout and password policies for users and used gpupdate /force to apply

![Client Setup](screenshots/account%20lockout%20policy.png)
![Client Setup](screenshots/password%20policy.png)

- Simulated an account unlock and password reset
![Client Setup](screenshots/unlock%20account%20+%20reset%20user%20password.png)

- Implemented a Group Policy Object which restricts user access to the Control Panel
![Client Setup](screenshots/control-panel-restriction)
