# AuroraPay Infrastructure

A project demonstrating secure, automated Azure infrastructure
for a fictional three-tier payment and utility-billing application.

## Project objectives

- Provision Azure infrastructure using Terraform.
- Design segmented virtual networks and least-privilege access.
- Deploy a containerized three-tier application to Azure Kubernetes Service.
- Implement an appropriate public entry point and web application firewall.
- Configure managed identities, monitoring, and security controls.
- Demonstrate autoscaling, deployment automation, and operational runbooks.
- Document cost controls, validation, limitations, and teardown procedures.

## Repository structure

- `app/` - Application components.
- `docs/` - Architecture, decisions, and operational runbooks.
- `infra/terraform/` - Terraform configuration and reusable modules.
- `kubernetes/` - Kubernetes manifests and environment overlays.
- `.github/workflows/` - CI/CD workflows.

## Security principles

- Never commit credentials, secrets, Terraform state, or plan files.
- Prefer managed identities and least-privilege permissions.
- Review Terraform plans before applying changes.
- Use private networking where appropriate.
- Apply cost controls and remove temporary resources when no longer needed.
