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
- Set up an Active Directory domain (JoshLab.local)
  
![Client Setup](screenshots/AD-domain.png)

![Client Setup](screenshots/local%20server%20info.png)

- Configured static IP addressing and DNS settings on both the server and client machines to enable communication
![Client Setup](screenshots/client-ip-config.png) ![Client Setup](screenshots/server-ip-config.png) 

- Confirmed the client machine was successfully joined to the domain via system properties
![Client Setup](screenshots/client-domain.png)

- Verified client-to-server connectivity and domain functionality using network diagnostic tools. Ping confirmed successful communication with the domain controller and nslookup validated proper DNS resolution for the domain.
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
- Set account lockout and password policies for domain users

![Client Setup](screenshots/account%20lockout%20policy.png)
![Client Setup](screenshots/password%20policy.png)

- Simulated an account unlock and password reset
![Client Setup](screenshots/unlock%20account%20+%20reset%20user%20password.png)

- Implemented a Group Policy Object which restricts user access to the Control Panel
![Client Setup](screenshots/control-panel-restriction.png)
