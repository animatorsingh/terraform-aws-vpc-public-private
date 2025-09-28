# AWS VPC with Public & Private Subnets using Terraform

This project provisions a complete AWS VPC setup with **Terraform**, including:

- ✅ Custom VPC (`10.0.0.0/16`)
- ✅ Public Subnet (`10.0.1.0/24`)
- ✅ Private Subnet (`10.0.2.0/24`)
- ✅ Internet Gateway for the public subnet
- ✅ NAT Gateway for the private subnet
- ✅ Security Group (allowing all traffic)
- ✅ EC2 instance in the **public subnet**
- ✅ EC2 instance in the **private subnet**

---

## 🏗 Architecture

- **Public Subnet (10.0.1.0/24)** → Has Internet Gateway → EC2 instance with public access.
- **Private Subnet (10.0.2.0/24)** → Routes traffic via NAT Gateway → EC2 instance without public IP.

---

## 🚀 How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/aws-vpc-terraform.git
   cd aws-vpc-terraform
terraform init
terraform plan
terraform apply
