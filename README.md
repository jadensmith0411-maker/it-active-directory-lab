# Active Directory Domain Services Lab (Windows Server)

## Overview
This project demonstrates the setup and configuration of an Active Directory Domain Services (AD DS) environment using a virtualized lab. The goal was to build a basic corporate-style domain with a Domain Controller, DNS, and a client machine joined to the domain.

This lab simulates real-world enterprise network administration tasks including domain creation, user management, and network configuration.

---

## Environment

- Virtualization Platform: Oracle VM VirtualBox
- Server OS: Windows Server (Domain Controller)
- Client OS: Windows 10/11
- Domain Services: Active Directory Domain Services (AD DS)
- DNS: Installed and configured on Domain Controller

---

## Network Configuration

The lab uses a dual-network adapter setup:

### Domain Controller
- Adapter 1: Internal Network (Lab Network)
  - Static IP configured (example: 192.168.x.x)
- Adapter 2: NAT (Internet Access)

### Client Machine
- Adapter 1: Internal Network (same as Domain Controller)
- Adapter 2: NAT (optional depending on lab requirements)

This allows:
- Internal domain communication between machines
- Internet access for updates and tools

---

## Active Directory Setup

### Domain Configuration
- Domain Name: (example: yourdomain.local)
- Server promoted to Domain Controller
- DNS role installed and integrated with AD DS

---

### Organizational Units (OUs)
Created basic structure:
- Users
- Computers
- Admins (if applicable)

---

### User Accounts
Created multiple domain users:
- Test User 1
- Test User 2
- Admin User

Users were assigned to appropriate OUs for organization and management.

---

## Client Machine Setup

- Joined client machine to the domain successfully
- Verified login using domain credentials
- Confirmed network connectivity with Domain Controller
- Tested domain authentication

---

## Key Skills Demonstrated

- Active Directory Domain Services (AD DS) installation and configuration
- DNS setup and integration with AD
- Virtual machine networking (Internal Network + NAT)
- Domain join process for client machines
- User and OU management in Active Directory
- Basic Windows Server administration

---

## Challenges & Fixes

- Issue: NAT/Internet not appearing in network settings  
  - Fix: Used NAT adapter in VirtualBox instead of “Internet” label

- Issue: Client not joining domain  
  - Fix: Verified DNS settings pointing to Domain Controller IP

---

## What I Learned

- How enterprise domains are structured and managed
- Importance of DNS in Active Directory environments
- How virtual networking impacts domain communication
- Troubleshooting domain join and connectivity issues

---

## Future Improvements

- Add Group Policy Objects (GPOs)
- Implement file sharing permissions across users
- Create multiple client machines
- Add PowerShell automation for user creation
- Simulate real enterprise role-based access control

---

## Author
- Name: [Your Name]
- Focus: IT / Systems / Active Directory / Networking
