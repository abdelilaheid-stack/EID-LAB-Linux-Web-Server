
# 🐍 EID LAB | Linux Web Server Infrastructure

![Status](https://img.shields.io/badge/STATUS-IN_PROGRESS-F0AD4E?style=for-the-badge)
![Platform](https://img.shields.io/badge/PLATFORM-KALI_LINUX-2374AB?style=for-the-badge)
![Project](https://img.shields.io/badge/PROJECT-CYBERSECURITY-168A62?style=for-the-badge)

## **Project Overview**

A hands-on Linux system administration and cybersecurity portfolio project using Kali Linux and VMware Workstation.

The project covers XFS storage, LVM, Apache, a custom EID website, a downloadable Python application, firewall configuration, network testing, and service troubleshooting.

## **Project Progress**

### ![Phase 01](https://img.shields.io/badge/PHASE_01-2374AB?style=for-the-badge) Environment Preparation
**Evidence: S01–S02**

- [x] Create GitHub repository
- [ ] Identify Kali Linux distribution, kernel, and hostname
- [ ] Configure hostname as eid-kali-server
- [ ] Inspect virtual disks and network interfaces
- [ ] Update package repositories and install project tools
- [ ] Capture S01: Kali environment and hostname
- [ ] Capture S02: Dedicated virtual disks

### ![Phase 02](https://img.shields.io/badge/PHASE_02-E67E22?style=for-the-badge) Standard Storage Configuration
**Evidence: S03–S04**

- [ ] Identify the correct unused virtual disk
- [ ] Create a 10 GiB partition
- [ ] Format the partition with XFS
- [ ] Capture S03: XFS partition
- [ ] Create the /eid-apps mount point
- [ ] Mount the XFS partition
- [ ] Create and verify a test file
- [ ] Capture S04: Mounted storage

### ![Phase 03](https://img.shields.io/badge/PHASE_03-8E44AD?style=for-the-badge) Logical Volume Management (LVM)
**Evidence: S05–S07**

- [ ] Identify the dedicated LVM virtual disk
- [ ] Create two 10 GiB partitions
- [ ] Capture S05: LVM partitions
- [ ] Initialize two Physical Volumes (PV)
- [ ] Create Volume Group (eid-vg)
- [ ] Create Logical Volume (abdul-webdata)
- [ ] Verify PV, VG, and LV
- [ ] Capture S06: LVM configuration
- [ ] Format the logical volume with XFS
- [ ] Mount it at /eid-content
- [ ] Create and verify a test file
- [ ] Capture S07: Mounted logical volume

### ![Phase 04](https://img.shields.io/badge/PHASE_04-C0392B?style=for-the-badge) Apache Web Server
**Evidence: S08–S09**

- [ ] Check Apache service status
- [ ] Start Apache
- [ ] Enable Apache at boot
- [ ] Verify Apache is active and enabled
- [ ] Capture S08: Apache service
- [ ] Test the default page at http://localhost
- [ ] Capture S09: Apache default page

### ![Phase 05](https://img.shields.io/badge/PHASE_05-168A62?style=for-the-badge) Build the Abdul EID Website
**Evidence: S10–S12**

- [ ] Create custom index.html homepage
- [ ] Capture S10: EID homepage
- [ ] Create python-app.html
- [ ] Develop the eid-guess.py number guessing game
- [ ] Verify Python syntax
- [ ] Capture S11: Python application
- [ ] Restart Apache
- [ ] Test homepage, application page, and download link
- [ ] Capture S12: Website navigation and downloads

### ![Phase 06](https://img.shields.io/badge/PHASE_06-B68A10?style=for-the-badge) Firewall Configuration
**Evidence: S13**

- [ ] Check UFW firewall status
- [ ] Review SSH access requirements before enabling UFW
- [ ] Allow HTTP traffic on TCP port 80
- [ ] Enable UFW
- [ ] Verify firewall rules
- [ ] Capture S13: Firewall configuration

### ![Phase 07](https://img.shields.io/badge/PHASE_07-566573?style=for-the-badge) Network Testing from EID-CLIENT
**Evidence: S14–S16**

- [ ] Prepare a second Linux VM on a reachable virtual network
- [ ] Verify connectivity to the EID server
- [ ] Scan TCP port 80 using Nmap
- [ ] Capture S14: Nmap scan
- [ ] Download eid-guess.py using curl
- [ ] Verify the downloaded file
- [ ] Capture S15: Application download
- [ ] Execute the Python game on the client
- [ ] Capture S16: Running Python game

### ![Phase 08](https://img.shields.io/badge/PHASE_08-B03A2E?style=for-the-badge) Troubleshooting Challenge
**Evidence: S17–S18**

- [ ] Simulate an Apache service outage
- [ ] Investigate service status and journal logs
- [ ] Capture S17: Service failure investigation
- [ ] Restore Apache service
- [ ] Verify service recovery and HTTP response
- [ ] Capture S18: Apache recovery

### ![Phase 09](https://img.shields.io/badge/PHASE_09-2471A3?style=for-the-badge) GitHub Portfolio Documentation
**Evidence: S19**

- [ ] Create the docs/ directory
- [ ] Document each implementation phase
- [ ] Add website source files
- [ ] Upload screenshots S01–S18
- [ ] Explain commands and verification results
- [ ] Document troubleshooting and lessons learned
- [ ] Review the completed repository
- [ ] Capture S19: GitHub portfolio

## **Technologies**

- Kali Linux
- VMware Workstation
- Linux CLI and systemd
- XFS and LVM
- Apache HTTP Server
- HTML and Python 3
- UFW Firewall
- Nmap and curl

## **Documentation Structure**

```text
EID-LAB-Linux-Web-Server/
├── README.md
├── docs/
│   ├── 01-environment.md
│   ├── 02-standard-storage.md
│   ├── 03-lvm-storage.md
│   ├── 04-apache-server.md
│   ├── 05-python-website.md
│   ├── 06-firewall.md
│   ├── 07-network-testing.md
│   └── 08-troubleshooting.md
├── website/
│   ├── index.html
│   ├── python-app.html
│   └── eid-guess.py
└── screenshots/
    └── S01–S19 (added after verification)
```

## **Project Status**

🚧 **In Progress**

Tasks and evidence will be updated as each phase is completed.

## **Author**

**Abdulelah Eid** | Cybersecurity Student
  
