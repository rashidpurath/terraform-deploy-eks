# Terraform EKS Cluster Deployment

This project provisions an **Elastic Kubernetes Service (EKS)** cluster on AWS using the official [terraform-aws-modules/eks/aws](https://github.com/terraform-aws-modules/terraform-aws-eks) module.

---

## 🔧 Project Structure

- **EKS Cluster**: `myapp-eks-cluster` using Terraform AWS module
- **VPC Module (Assumed)**: Provides private subnets and VPC ID for the EKS module
- **Managed Node Group**: 3 `t2.small` instances for development use

---

## 📁 Files

- `main.tf` — Main Terraform configuration
- `vpc.tf` — Contains VPC and subnet definitions (must output `vpc_id` and `private_subnets`)
- `eks-cluster.tf` — Defines the EKS cluster module
- `nginx-config.yaml` — Example Kubernetes manifest
- `README.md` — You're reading it 😎

---

## 🚀 How to Use

### 1. Clone the Repository
```bash
git clone https://gitlab.com/<your-username>/terraform-deploy-eks.git
cd terraform-deploy-eks

