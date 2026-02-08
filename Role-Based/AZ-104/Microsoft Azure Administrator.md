# AZ-104 Readiness Checklist (Azure Administrator)

Use this checklist to confirm **operational readiness** and **exam alignment**.

---

## 👤 Manage Azure Identities and Governance (20–25%)

### Microsoft Entra users and groups
- [ ] Create users and groups
- [ ] Manage user and group properties
- [ ] Assign and manage licenses
- [ ] Manage external (guest) users
- [ ] Configure self-service password reset (SSPR)

---

### Access to Azure resources
- [ ] Understand built-in Azure roles
- [ ] Assign roles at different scopes (MG, subscription, RG, resource)
- [ ] Interpret effective access and role assignments

---

### Subscriptions and governance
- [ ] Implement and manage Azure Policy
- [ ] Configure resource locks (ReadOnly, Delete)
- [ ] Apply and manage tags
- [ ] Create and manage resource groups
- [ ] Create and manage subscriptions
- [ ] Configure management groups
- [ ] Manage costs using:
  - [ ] Budgets
  - [ ] Cost alerts
  - [ ] Azure Advisor recommendations

---

## 💾 Implement and Manage Storage (15–20%)

### Storage access and security
- [ ] Configure Storage firewalls and VNets
- [ ] Create and use SAS tokens
- [ ] Configure stored access policies
- [ ] Manage access keys
- [ ] Configure identity-based access for Azure Files

---

### Storage accounts
- [ ] Create and configure storage accounts
- [ ] Configure redundancy (LRS, ZRS, GRS, GZRS)
- [ ] Configure object replication
- [ ] Configure encryption (Microsoft-managed, CMK)
- [ ] Manage data using Azure Storage Explorer
- [ ] Manage data using AzCopy

---

### Azure Files and Blob Storage
- [ ] Create and configure file shares
- [ ] Create and configure blob containers
- [ ] Configure storage tiers
- [ ] Configure soft delete (blobs and containers)
- [ ] Configure snapshots and soft delete for Azure Files
- [ ] Configure blob lifecycle management
- [ ] Configure blob versioning

---

## 🖥️ Deploy and Manage Azure Compute Resources (20–25%)

### ARM / Bicep
- [ ] Interpret ARM templates
- [ ] Interpret Bicep files
- [ ] Modify existing ARM templates
- [ ] Modify existing Bicep files
- [ ] Deploy resources using ARM or Bicep
- [ ] Export deployments as ARM templates
- [ ] Convert ARM templates to Bicep

---

### Virtual machines
- [ ] Create virtual machines
- [ ] Configure Azure Disk Encryption
- [ ] Move VMs between resource groups, subscriptions, or regions
- [ ] Manage VM sizes
- [ ] Manage VM disks
- [ ] Deploy VMs to availability zones
- [ ] Deploy VMs to availability sets

---

### Virtual Machine Scale Sets
- [ ] Deploy VM Scale Sets
- [ ] Configure scaling rules
- [ ] Manage instances

---

### Containers
- [ ] Create and manage Azure Container Registry (ACR)
- [ ] Provision containers using Azure Container Instances
- [ ] Provision containers using Azure Container Apps
- [ ] Configure sizing and scaling for containers

---

### Azure App Service
- [ ] Provision App Service plans
- [ ] Configure scaling for App Service plans
- [ ] Create App Services
- [ ] Configure certificates and TLS
- [ ] Map custom DNS names
- [ ] Configure backups
- [ ] Configure networking settings
- [ ] Configure deployment slots

---

## 🌐 Implement and Manage Virtual Networking (15–20%)

### Virtual networks
- [ ] Create and configure VNets and subnets
- [ ] Configure VNet peering
- [ ] Configure public IP addresses
- [ ] Configure user-defined routes (UDRs)
- [ ] Troubleshoot network connectivity

---

### Secure access
- [ ] Create and configure NSGs
- [ ] Create and configure Application Security Groups (ASGs)
- [ ] Evaluate effective NSG security rules
- [ ] Implement Azure Bastion

---

### PaaS networking
- [ ] Configure service endpoints
- [ ] Configure private endpoints

---

### Name resolution and load balancing
- [ ] Configure Azure DNS
- [ ] Configure public load balancers
- [ ] Configure internal load balancers
- [ ] Troubleshoot load balancing issues

---

## 📊 Monitor and Maintain Azure Resources (10–15%)

### Azure Monitor
- [ ] Interpret metrics
- [ ] Configure diagnostic log settings
- [ ] Query and analyze logs
- [ ] Configure alert rules
- [ ] Configure action groups
- [ ] Configure alert processing rules

---

### Azure Monitor Insights
- [ ] Monitor virtual machines
- [ ] Monitor storage accounts
- [ ] Monitor networks

---

### Network diagnostics
- [ ] Use Azure Network Watcher
- [ ] Use Connection Monitor

---

### Backup and recovery
- [ ] Create a Recovery Services vault
- [ ] Create an Azure Backup vault
- [ ] Create and configure backup policies
- [ ] Perform backup and restore operations
- [ ] Configure Azure Site Recovery
- [ ] Perform failover to a secondary region
- [ ] Interpret backup reports and alerts

---

## ✅ Final Readiness Check

You are ready for AZ-104 when you can:
- [ ] Confidently operate Azure resources via Portal, CLI, or PowerShell
- [ ] Troubleshoot identity, networking, and storage issues
- [ ] Explain governance decisions (Policy, RBAC, Locks)
- [ ] Interpret monitoring data and act on alerts
- [ ] Perform backup, restore, and failover scenarios