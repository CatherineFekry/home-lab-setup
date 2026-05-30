# Home Lab Setup - Windows Server 2022 & Active Directory

## Overview
Built a complete home lab environment using VMware Workstation to simulate a real enterprise IT environment, demonstrating hands-on experience with Windows Server administration.

## Environment
- **Server:** Windows Server 2022 (Domain Controller - DC-01) | IP: 192.168.1.10
- **Client:** Windows 10 (HELPDESK-01) | IP: 192.168.1.20

## Skills Demonstrated

### Active Directory
- Installed and configured AD DS
- Promoted server to Domain Controller (lab.local)
- Created Users, Groups, and Organizational Units (OUs)
- Reset passwords via AD

### Network
- Configured static IP addresses
- Troubleshot VM network issue (NAT vs Custom VMnet0)
- Set up DNS server

### Group Policy (GPO)
- Created GPO to block USB access on all domain machines

### DHCP
- Installed DHCP Server
- Configured scope: 192.168.1.50 - 192.168.1.100

### Remote Access
- Enabled and tested Remote Desktop (RDP) between VMs
- Accessed Server Manager remotely from Windows 10 client

### File Sharing
- Created and accessed shared folder (IT-Share) across the network

## Troubleshooting Case
**Problem:** Windows 10 client could not join domain (ERROR_TIMEOUT)
**Root Cause:** VMs were on different VMware networks (NAT vs Custom)
**Solution:** Changed both VMs to Custom VMnet0 and set static IP + DNS
**Result:** Client successfully joined lab.local domain
