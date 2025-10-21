# 🛡️ Automated IAM & VPC Infrastructure using Terraform + LocalStack

This project demonstrates how to automatically provision and secure a simulated AWS cloud infrastructure 
using **Terraform** integrated with **LocalStack** (a local AWS emulator).  
It aims to replicate and analyze AWS IAM, VPC, EC2, and Security Group configurations to study compliance with **CIS AWS Foundations Benchmark**.

---

## 🚀 Features
- Automated creation of IAM Users.
- Custom VPC setup with Internet Gateway, Subnet, and Route Tables.
- Secure Security Group configuration (SSH, HTTP, HTTPS).
- Auto-deployed EC2 instance running Apache Web Server.
- Integration with LocalStack for local AWS simulation.
- Infrastructure output for monitoring (Public/Private IPs, IDs).

---

## 🧠 Purpose
This repository is part of my research project:
> **“Pengembangan Tool Otomatisasi Audit Kepatuhan IAM AWS Sederhana Menggunakan Terraform dan Python Berdasarkan 10 Aturan Krusial CIS Benchmark.”**

It serves as an experimental infrastructure to automate configuration, test compliance, 
and build a foundation for security auditing in cloud-based systems.

---

## ⚙️ Tech Stack
- **Terraform** – Infrastructure as Code (IaC)
- **LocalStack** – Local AWS cloud emulator
- **Python (Boto3)** – For security and compliance testing scripts *(future stage)*
- **AWS CLI** – Command-line management

---

## 🧩 Usage
### 1️⃣ Run LocalStack
localstack start

2️⃣ Initialize Terraform
terraform init

3️⃣ Deploy Infrastructure
terraform apply -auto-approve

4️⃣ Verify Resources
aws --endpoint-url=http://localhost:4566 iam list-users

🧾 Outputs

Terraform will display the following:

✅ IAM User ID

🌐 Public IP of the web server

🔒 Security Group details

🧩 VPC and Subnet IDs

📘 Author

Haydar Aulia Rahman
Student of Informatics, Universitas Muhammadiyah Surakarta
Focus: Cyber Security & Cloud Infrastructure
📫 LinkedIn
 | GitHub


