# CMIT 495 - Project 2: Cloud Computing

**Student:** Aron Michaels  
**Date:** March 25, 2026  
**Course:** CMIT 495 Current Trends and Projects in Computer Networks and Security

## Project Overview
I provisioned a **Windows Server 2022** virtual machine in AWS EC2, connected using Remote Desktop (RDP), launched an **Ubuntu 24.04 LTS** server, created and mounted an **Amazon Elastic File System (EFS)**, uploaded proof to an **Amazon S3** bucket, and terminated all resources.

This demonstrates **PaaS** cloud computing, secure remote access, shared storage, and best practices.

## Skills Demonstrated
- AWS EC2 Windows + Linux provisioning
- RDP with decrypted password
- SSH via PuTTY
- EFS creation & NFSv4.1 mounting
- Security group configuration (RDP, SSH, NFS)
- S3 object upload
- Resource cleanup

## Files
- [Project2-Cloud-Computing-Aron.pdf](Project2-Cloud-Computing-Aron.pdf) ← Full assignment
- `/screenshots` folder with every step

## Key Learning Outcomes & Lessons Learned
- NIST cloud characteristics (on-demand self-service, rapid elasticity, measured service) in action.
- EFS is managed shared storage — I learned the hard way that **every** EFS mount target must use the exact same security group with NFS port 2049 allowed.
- Lesson: Always verify mount targets and security groups before running the mount command.

## Screenshots Gallery

![01. AWS Dashboard](<img width="1903" height="926" alt="screenshot01-dashboard" src="https://github.com/user-attachments/assets/dd231048-5f2a-4bcb-b22d-788f5b6c4875" />)  
![02. Windows Name & Tags](<img width="1902" height="825" alt="screenshot02-windows-name-tags" src="https://github.com/user-attachments/assets/4ece74a1-ad14-47ec-a0d4-412af4cdf72e" />)  
![03. Windows AMI Selection]( <img width="1883" height="802" alt="screenshot03-windows-ami" src="https://github.com/user-attachments/assets/4ce7d3ea-2c05-40d6-a628-8be72ca3e7d8" />)  
![04. Windows Instance Type](<img width="1910" height="821" alt="screenshot04-windows-type" src="https://github.com/user-attachments/assets/c79d5a51-83b7-4346-8895-19bda71c96b5" />)  
![05. Windows Key Pair Creation](<img width="1908" height="828" alt="screenshot05-windows-key-pair" src="https://github.com/user-attachments/assets/9eea9ae0-37ce-4140-a8b4-2a8f51bf1304" />)  
![06. Windows Key Pair PEM Download](<img width="1898" height="998" alt="screenshot06-windows-key-pair-pem" src="https://github.com/user-attachments/assets/bf120ed3-8309-43d3-9fae-f695bba5bf87" />)  
![07. Get Windows Password](<img width="1897" height="812" alt="screenshot07-get-windows-password (2)" src="https://github.com/user-attachments/assets/0107c2c7-9ffc-4ae4-a9d7-773f25077ad4" />)  
![08. Decrypt Windows Password](<img width="1905" height="881" alt="screenshot08-decrypt-windows-password" src="https://github.com/user-attachments/assets/d1a54d93-99dd-4027-a49c-dc096302a216" />)  
![09. Windows Desktop]( <img width="1669" height="939" alt="screenshot09-windows-desktop" src="https://github.com/user-attachments/assets/c9a4f7c7-dd1b-41b1-8df8-375fc7586f53" />)  
![10. EFS Created](<img width="1846" height="640" alt="screenshot10-efs-created" src="https://github.com/user-attachments/assets/fc95edb0-3449-4c50-962d-f8df66496d9b" />)  
![11. EFS Mounted with 1GiB Test File](<img width="646" height="395" alt="screenshot11-efs-mounted-1gib" src="https://github.com/user-attachments/assets/d41d3ad5-d7df-4c14-a9cd-7492d944410b" />)  
![12. S3 Upload Success](<img width="1828" height="744" alt="screenshot12-s3-upload" src="https://github.com/user-attachments/assets/b2e8145c-1452-4dd5-9ceb-e3bcdf6f3597" />)

⭐ Completed as part of UMGC CMIT 495. Open to feedback!
