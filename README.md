# 🚀 Terraform + Ansible LEMP Deployment on AWS

This project demonstrates end-to-end Infrastructure Automation using **Terraform** and **Ansible** to deploy a complete LEMP stack (Linux, Nginx, MariaDB, PHP) on an AWS EC2 instance.

It represents a real-world DevOps workflow combining Infrastructure as Code (IaC) and Configuration Management.

---

## 📌 Project Overview

This project automates:

- Provisioning AWS EC2 infrastructure using Terraform
- Configuring the server using Ansible
- Installing a complete LEMP stack
- Deploying a custom static web page
- Making the website accessible via public IP

---

## 🏗️ Architecture Workflow

```text
Developer
   │
   ▼
Terraform (Infrastructure as Code)
   │
   ▼
AWS EC2 Instance Created
   │
   ▼
Terraform Output (Public IP)
   │
   ▼
Ansible (Configuration Management)
   │
   ▼
Install Nginx + MariaDB + PHP
   │
   ▼
Deploy index.html
   │
   ▼
Website Live on Browser
🛠️ Tech Stack

- AWS EC2

- Terraform

- Ansible

- Ubuntu 24.04

- Nginx

- MariaDB

- PHP

- Git & GitHub

📂 Project Structure
terraform-ansible-lemp-aws/
│
├── terraform/
│   ├── main.tf
│   ├── variables.tf
│   └── outputs.tf
│
├── ansible/
│   ├── lemp.yml
│   └── inventory
│
├── index.html
├── screenshots/
│   └── project-output.png
└── README.md

🚀 Deployment Steps
1️⃣ Clone Repository
git clone https://github.com/Aditikl/terraform-ansible-lemp-aws.git
cd terraform-ansible-lemp-aws

2️⃣ Provision Infrastructure
cd terraform
terraform init
terraform apply

Terraform will create an EC2 instance and output the public IP.

3️⃣ Configure Server
cd ../ansible
ansible-playbook -i inventory lemp.yml

This installs:

- Nginx

- MariaDB

- PHP

- Deploys index.html

📸 Project Output

<img width="1918" height="877" alt="Screenshot 2026-02-21 150222" src="https://github.com/user-attachments/assets/6dec1501-f750-4381-9627-bcd55518fb66" />





🎯 Key Learnings

- Infrastructure as Code (IaC)

- Terraform state management

- Configuration management using Ansible

- SSH-based automation

- Cloud provisioning workflow

- End-to-end DevOps implementation

🔐 Security Best Practices

The following files are excluded using .gitignore:

 terraform.tfstate

.terraform/

*.pem files

Sensitive credentials


👩‍💻 Author

Aditi Kulkarni
B.Tech (Electronics & Telecommunication)
Aspiring DevOps Engineer

⭐ If you found this project useful, feel free to star the repository!
