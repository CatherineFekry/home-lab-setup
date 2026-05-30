# Home Lab Setup - Windows Server 2022 & Active Directory

## Overview
Built a home lab environment using VMware Workstation to simulate a real enterprise IT environment.

## Environment
- Windows Server 2022 (Domain Controller - DC-01)
- Windows 10 Client (HELPDESK-01)

## What I configured
- Active Directory Domain Services (AD DS)
- Domain Controller setup (lab.local)
- Joined Windows 10 client to the domain
- Created Users and Groups in AD
- Password Reset via AD
- Group Policy (Block USB)
- DHCP Server with scope 192.168.1.50-100
- Shared Folder (IT-Share)
- Remote Desktop between VMs
- Troubleshot network issue (NAT vs Custom VMnet0)
