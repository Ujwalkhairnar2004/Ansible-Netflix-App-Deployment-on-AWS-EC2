📌 Project Overview

This project demonstrates how to use Ansible to deploy a Netflix Clone application across multiple AWS EC2 environments.

Infrastructure includes separate Development and Testing servers, managed from a central Ansible control node using YAML playbooks.

The goal of this project is to showcase:

Configuration management with Ansible

Environment separation (Dev & Test)

Automated application deployment

Infrastructure provisioning best practices

🏗️ Architecture
Servers Created

dev1 (EC2)

dev2 (EC2)

test1 (EC2)

test2 (EC2)

Ansible Control Node

<img width="1366" height="768" alt="{DA94ABD4-E407-4AF4-B529-F60ABB10B06A}" src="https://github.com/user-attachments/assets/3f029a7a-6575-4687-b0fc-06d7cf58ba07" />


Environments

Development Environment → dev1, dev2

Testing Environment → test1, test2

All servers are connected to the Ansible control node using SSH.

⚙️ Technologies Used

AWS EC2

Ansible

YAML Playbooks

Linux (Ubuntu)

Git & GitHub

Netflix Clone Application (Frontend)

📁 Project

<img width="1366" height="768" alt="{DB655AA8-5C8D-4A29-B9B8-17937EADD996}" src="https://github.com/user-attachments/assets/2912c80f-4232-44a2-8aab-dd6961c661e7" />

🔑 Prerequisites

AWS account

5 EC2 instances created

SSH key configured

Ansible installed on control node

Git installed

Install Ansible:

sudo dnf install Ansible -y

🧾 Inventory Configuration

Example hosts file:

[dev]

dev1 ansible_host=<DEV1_IP>

dev2 ansible_host=<DEV2_IP>

[test]

test1 ansible_host=<TEST1_IP>

test2 ansible_host=<TEST2_IP>

<img width="1366" height="768" alt="{C96A8583-F44C-4FC4-A65F-F3333824E05B}" src="https://github.com/user-attachments/assets/8a662e75-34ab-4459-baa6-f4012d78d916" />

🚀 Deployment 

[test]

<img width="1366" height="768" alt="{559C3F75-F0A6-412B-87CE-5AFC557D68F3}" src="https://github.com/user-attachments/assets/9abf7678-1d42-4337-9505-70c78a056f63" />

[dev]

<img width="1366" height="768" alt="{A2694035-5813-402D-8B05-FCF4F6BA564C}" src="https://github.com/user-attachments/assets/2d090b07-d720-4c95-b23c-0b85a5a976ba" />

This playbook will:

Install dependencies

Copy Netflix clone code

Configure web server

Start application

📜 Example Playbook Tasks

Install Nginx

Copy application files

Set permissions

Start services

✅ Result

After successful deployment:

Dev environment runs Netflix clone

Test environment runs Netflix clone

Application accessible via EC2 public IP

<img width="1366" height="768" alt="{5C861D0F-5621-4A5D-AB7B-C20809B198D6}" src="https://github.com/user-attachments/assets/dda78cb9-9e51-438a-a5c0-a84c870a4db3" />

🎥 Demo Videos

You can watch the deployment process in the following videos:



👨‍💻 Author

Ujwal Ganesh Khairnar





















