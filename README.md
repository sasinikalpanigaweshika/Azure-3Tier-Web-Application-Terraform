# Azure 3-Tier Web Application using Terraform

A production-grade three-tier web application deployed on Microsoft Azure using Terraform (IaC).

## Tech Stack
- Terraform (IaC)
- Azure (VM Scale Sets, App Gateway, WAF, Key Vault, PostgreSQL)
- Docker + Docker Hub
- GitHub Actions (CI/CD)
- Node.js (Frontend)
- Go (Backend)
- PostgreSQL (Database)

## CI/CD Pipeline
GitHub Actions automatically:
- Builds Docker images for frontend and backend
- Pushes images to Docker Hub on every commit to main branch

## Infrastructure
- Application Gateway + WAF (OWASP 3.2)
- VM Scale Sets with auto-scaling
- Private subnets + NSGs
- Azure Bastion
- Azure Key Vault
- PostgreSQL with read replica
- Private DNS Zones
- Remote Terraform state in Azure Blob Storage
