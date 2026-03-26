# CMIT 495 - Project 2: Cloud Computing

**Student:** Aron 
**Date:** March 25, 2026  
**Course:** CMIT 495 Current Trends and Projects in Computer Networks and Security

## Project Overview
I provisioned a **Windows Server 2022** virtual machine in AWS EC2, connected to it using Remote Desktop (RDP), launched an **Ubuntu 24.04 LTS** server, created an **Amazon Elastic File System (EFS)**, mounted it to the Ubuntu instance, created a 1 GiB test file to prove shared storage, uploaded proof to an **Amazon S3** bucket, and properly terminated all resources.

This project demonstrates **PaaS** cloud computing, secure remote access, shared network file systems, and object storage — all while following AWS best practices and the shared responsibility model.

## Skills Demonstrated
- AWS EC2 Windows and Linux instance provisioning
- RDP remote access with decrypted Administrator password
- SSH access via PuTTY
- Amazon EFS creation and NFSv4.1 mounting
- Security group configuration (RDP, SSH, NFS)
- Amazon S3 bucket creation and file upload
- Proper resource cleanup (termination) to avoid charges
- Documentation with screenshots and step-by-step explanations

## Files
- [Project2-Cloud-Computing-Aron.pdf](Project2-Cloud-Computing-Aron.pdf) ← Full assignment with all screenshots and explanations
- `/screenshots` folder containing every step

## Key Learning Outcomes & Lessons Learned
- **Cloud computing** (per NIST) gives on-demand self-service, rapid elasticity, and measured service — I saw this live when launching VMs in minutes.
- EFS is a **managed NFS** service that lets multiple VMs share files — super useful for real-world apps.
- **Biggest struggle**: Security groups and mount targets — I had to make sure **every** EFS mount target used the exact same security group with NFS port 2049 allowed. Once I fixed that, the mount worked instantly.
- Lesson: Always double-check “My IP” rules and mount-target attachments before connecting.
- This project directly supports my goal of moving from call-center work into entry-level cybersecurity/IT roles.

## Screenshots Gallery

![01. AWS Dashboard](screenshots/screenshot01-dashboard.png)  
![02. Windows Name & Tags](screenshots/screenshot02-windows-name-tags.png)  
![03. Windows AMI Selection](screenshots/screenshot03-windows-ami.png)  
![04. Windows Instance Type](screenshots/screenshot04-windows-type.png)  
![05. Windows Key Pair Creation](screenshots/screenshot05-windows-key-pair.png)  
![06. Windows Key Pair PEM Download](screenshots/screenshot06-windows-key-pair-pem.png)  
![07. Get Windows Password](screenshots/screenshot07-get-windows-password.png)  
![08. Decrypt Windows Password](screenshots/screenshot08-decrypt-windows-password.png)  
![09. Windows Desktop](screenshots/screenshot09-windows-desktop.png)  
![10. EFS Created](screenshots/screenshot10-efs-created.png)  
![11. EFS Mounted with 1GiB Test File](screenshots/screenshot11-efs-mounted-1gib.png)  
![12. S3 Upload Success](screenshots/screenshot12-s3-upload.png)

⭐ This project was completed as part of the UMGC CMIT 495 program. Open to feedback or collaboration!
Add final README.md for Project 2 portfolio
