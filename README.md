# Home Network Setup & Security Hardening (VMware Workstation)

## Project Overview
This project simulates a small business network using VMware Workstation to demonstrate foundational networking and cybersecurity skills.  
It includes static IP configuration, subnetting, firewall rules, WPA3 router security, and system hardening on Windows and Linux virtual machines.


---

## Objectives 
- Build a private network using VMware Workstation (VMnet2)
- Configure static IPs and verify connectivity
- Apply network and host-based firewalls
- Implement WPA3 encryption and disable insecure router settings
- Document and test network security controls

---

## Tools & Technologies 
- VMware Workstation  
- Windows 10/11  
- Ubuntu Server  
- pfSense (optional firewall/router)  
- Windows Defender Firewall / UFW  
- Wireshark (for verification) 


---

## Network Topology
| Device | Role | IP Address | OS |
|---------|------|-------------|----|
| VM1 | Workstation | 192.168.50.20 | Windows 10 |
| VM2 | Server | 192.168.50.10 | Ubuntu Server |
| VM3 | Router/Firewall | 192.168.50.1 | pfSense (optional) |



---

## Configuration Summary
### Static IP Setup
```bash
# Ubuntu
sudo nano /etc/netplan/00-installer-config.yaml
# Assigned IP 192.168.50.10
