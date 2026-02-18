# Active Directory Deployment Lab

This is a hands-on lab demonstrating the provisioning of an EC2 instance and configuring **Active Directory Domain Services (AD DS)**.

# Watch me do the lab HERE

https://www.loom.com/share/a7b1a8efe2e3492d85ba8535cb490841 

## Objective

The purpose of this project was to:

- Provision a Windows Server EC2 instance
- Install and configure Active Directory Domain Services
- Configure a new forest and domain

## Tools

| Component              | Configuration                         |
|------------------------|---------------------------------------|
| Cloud Provider         | AWS                                   |
| Compute Service        | Amazon EC2                            |
| Operating System       | Windows Server Base 2025              |
| Directory Service      | Active Directory Domain Services      |


## Steps

1. Launching an EC2 instance
  - Click Launch Instance.
  <img width="1179" height="383" alt="Screenshot 2026-02-17 at 10 25 23 PM" src="https://github.com/user-attachments/assets/c87a480b-d47f-4556-a98d-41989652e0e6" />

  - Name your instance and select the Windows Server Base 2025 AMI.
  <img width="863" height="545" alt="Screenshot 2026-02-17 at 10 26 30 PM" src="https://github.com/user-attachments/assets/15d2d3de-306a-4268-a15f-a830131f55d9" />

  - Create a new key pair and save it.
  <img width="482" height="474" alt="Screenshot 2026-02-17 at 10 27 21 PM" src="https://github.com/user-attachments/assets/31ca09d0-3a62-4e65-b5b6-53ba98dc7dda" />

  - Download RDP file, decrypt the password using the new key pair and login to the VM.
  <img width="1297" height="495" alt="Screenshot 2026-02-17 at 10 28 49 PM" src="https://github.com/user-attachments/assets/35de701e-5661-4b84-8e9a-857265eaf03a" />

2. Configure Active Directory
  - Open Server manager in the VM.
    <img width="641" height="719" alt="Screenshot 2026-02-17 at 10 35 48 PM" src="https://github.com/user-attachments/assets/2fd52cf4-2ea4-401d-bc75-cbe2a516d11c" />

  - Click Add Roles and Features.
    <img width="785" height="556" alt="Screenshot 2026-02-17 at 10 37 57 PM" src="https://github.com/user-attachments/assets/0cdf5d06-b867-47bd-8ee7-a26544d06e42" />

  - Click next until Features section, add Active Directory Domain Services and install it.
    <img width="415" height="433" alt="Screenshot 2026-02-17 at 10 38 34 PM" src="https://github.com/user-attachments/assets/f64a2002-8698-4df8-95e4-753b525f7273" />
    <img width="785" height="558" alt="Screenshot 2026-02-17 at 10 39 00 PM" src="https://github.com/user-attachments/assets/d3d143e6-d674-4fb1-89f8-e242adffd512" />
    <img width="788" height="557" alt="Screenshot 2026-02-17 at 10 44 26 PM" src="https://github.com/user-attachments/assets/35a5b2cd-4740-474c-a8c8-04a40af426d7" />

  - Click the flag on the top right corner, and select promote this server to domain controller.
    <img width="343" height="322" alt="Screenshot 2026-02-17 at 10 44 36 PM" src="https://github.com/user-attachments/assets/d7d9f123-7c46-49e0-8787-e8807525c3e0" />

  - Add a new forest, create a password, and click install.
    <img width="762" height="560" alt="Screenshot 2026-02-17 at 10 50 16 PM" src="https://github.com/user-attachments/assets/48616048-5014-462c-b7f5-9f6ea8f1f006" />
    <img width="760" height="559" alt="Screenshot 2026-02-17 at 10 50 54 PM" src="https://github.com/user-attachments/assets/bfd274f0-967e-4ac9-833e-bdfbc238420f" />
    <img width="761" height="560" alt="Screenshot 2026-02-17 at 10 55 51 PM" src="https://github.com/user-attachments/assets/96520a73-ef4d-4ba9-bdb6-c7a35302c757" />

  - After installation is complete, it will prompt to restart. Once restarted, Active Directory will be enabled on this VM.
    <img width="612" height="210" alt="Screenshot 2026-02-17 at 11 01 41 PM" src="https://github.com/user-attachments/assets/a0d1da11-b235-402d-831d-ca7a48be254a" />

## Outcome

Successfully depolying EC2 instance on AWS and configuring Active Directory Domain Services on a Windows server.
