# Azure ACR Security Guardrails

This repository contains the target configuration and SRE runtime files compiled by the **Azure ACR Security Guardrails** dashboard module.

## 🚀 Description
Secure Azure Container Registries. Generate ACR access controls, content trust validation settings, image signing tasks, and Defender security triggers.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/infra/acr/acr_policy.tf`
- **Execution Command**: `terraform init && terraform apply -auto-approve`
- **Validation Command**: `terraform show`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-azure-acr-secure.git
   cd tp-azure-acr-secure
   ```

2. **Run Execution Target:**
   ```bash
   terraform init && terraform apply -auto-approve
   ```

3. **Verify Runtime Stability:**
   ```bash
   terraform show
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
