# AZ-104

## Skills at a glance

<https://learn.microsoft.com/en-gb/training/paths/az-104-administrator-prerequisites/>

- Manage Azure identities and governance (20–25%)
- Implement and manage storage (15–20%)
- Deploy and manage Azure compute resources (20–25%)
- Implement and manage virtual networking (15–20%)
- Monitor and maintain Azure resources (10–15%)

## Manage Azure identities and governance (20–25%)

<https://learn.microsoft.com/en-gb/credentials/certifications/resources/study-guides/az-104#manage-azure-identities-and-governance-2025>

<https://learn.microsoft.com/en-gb/training/paths/az-104-manage-identities-governance/>

### Manage Microsoft Entra users and groups

- Create users and groups
- Manage user and group properties
- Manage licenses in Microsoft Entra ID
- Manage external users
- Configure self-service password reset (SSPR)

### Manage access to Azure resources

- Manage built-in Azure roles
- Assign roles at different scopes
- Interpret access assignments

### Manage Azure subscriptions and governance

- Implement and manage Azure Policy
- Configure resource locks
- Apply and manage tags on resources
- Manage resource groups
- Manage subscriptions
- Manage costs by using alerts, budgets, and Azure Advisor recommendations
- Configure management groups

## Implement and manage storage (15–20%)

<https://learn.microsoft.com/en-gb/credentials/certifications/resources/study-guides/az-104#implement-and-manage-storage-1520>

<https://learn.microsoft.com/en-gb/training/paths/az-104-manage-storage/>

### Configure access to storage

- Configure Azure Storage firewalls and virtual networks
- Create and use shared access signature (SAS) tokens
- Configure stored access policies
- Manage access keys
- Configure identity-based access for Azure Files

### Configure Azure Files and Azure Blob Storage

- Create and configure a file share in Azure Files
- Create and configure a container in Azure Blob Storage
- Configure storage tiers
- Configure soft delete for blobs and containers
- Configure snapshots and soft delete for Azure Files
- Configure blob lifecycle management
- Configure blob versioning

## Deploy and manage Azure compute resources (20–25%)

<https://learn.microsoft.com/en-gb/credentials/certifications/resources/study-guides/az-104#deploy-and-manage-azure-compute-resources-2025>

<https://learn.microsoft.com/en-gb/training/paths/az-104-manage-compute-resources/>

### Automate deployment of resources by using Azure Resource Manager (ARM) templates or Bicep files

- Interpret an Azure Resource Manager template or a Bicep file
- Modify an existing Azure Resource Manager template
- Modify an existing Bicep file
- Deploy resources by using an Azure Resource Manager template or a Bicep file
- Export a deployment as an Azure Resource Manager template or convert an Azure Resource Manager template to a Bicep file

### Create and configure virtual machines

- Create a virtual machine
- Configure encryption at host for Azure virtual machines
- Move a virtual machine to another resource group, subscription, or region
- Manage virtual machine sizes
- Manage virtual machine disks
- Deploy virtual machines to availability zones and availability sets
- Deploy and configure an Azure Virtual Machine Scale Sets

### Provision and manage containers in the Azure portal

- Create and manage an Azure Container Registry
- Provision a container by using Azure Container Instances
- Provision a container by using Azure Container Apps
- Manage sizing and scaling for containers, including Azure Container Instances and Azure Container Apps

### Create and configure Azure App Service

- Provision an App Service plan
- Configure scaling for an App Service plan
- Create an App Service
- Configure certificates and Transport Layer Security (TLS) for an App Service
- Map an existing custom DNS name to an App Service
- Configure backup for an App Service
- Configure networking settings for an App Service
- Configure deployment slots for an App Service

## Implement and manage virtual networking (15–20%)

<https://learn.microsoft.com/en-gb/credentials/certifications/resources/study-guides/az-104#implement-and-manage-virtual-networking-1520>

<https://learn.microsoft.com/en-gb/training/paths/az-104-manage-virtual-networks/>

### Configure and manage virtual networks in Azure

- Create and configure virtual networks and subnets
- Create and configure virtual network peering
- Configure public IP addresses
- Configure user-defined routes
- Troubleshoot network connectivity

###  Configure secure access to virtual networks

- Create and configure network security groups (NSGs) and application security groups
- Evaluate effective security rules in NSGs
- Implement Azure Bastion
- Configure service endpoints for Azure platform as a service (PaaS)
- Configure private endpoints for Azure PaaS

### Configure name resolution and load balancing

- Configure Azure DNS
- Configure an internal or public load balancer
- Troubleshoot load balancing

## Monitor and maintain Azure resources (10–15%)

<https://learn.microsoft.com/en-gb/credentials/certifications/resources/study-guides/az-104#monitor-and-maintain-azure-resources-1015>

<https://learn.microsoft.com/en-gb/training/paths/az-104-monitor-backup-resources/>

### Monitor resources in Azure

- Interpret metrics in Azure Monitor
- Configure log settings in Azure Monitor
- Query and analyze logs in Azure Monitor
- Set up alert rules, action groups, and alert processing rules in Azure Monitor
- Configure and interpret monitoring of virtual machines, storage accounts, and networks by using Azure Monitor Insights
- Use Azure Network Watcher and Connection monitor

### Implement backup and recovery

- Create a Recovery Services vault
- Create an Azure Backup vault
- Create and configure a backup policy
- Perform backup and restore operations by using Azure Backup
- Configure Azure Site Recovery for Azure resources
- Perform a failover to a secondary region by using Site Recovery
- Configure and interpret reports and alerts for backups

## Gotcha's

| Area               | What repeatedly catches candidates                                                                                                              |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| RBAC               | Scope inheritance; assigning at management-group, subscription, resource-group or resource scope; difference between Entra roles and Azure RBAC |
| Governance         | Policy versus initiatives, locks versus RBAC, remediation and managed identities, tag inheritance not occurring automatically                   |
| Entra ID           | Which features require P1/P2; group membership types; dynamic groups; administrative units; external users                                      |
| Networking         | Peering is non-transitive; effective routes; longest-prefix routing; NSG evaluation; service endpoints versus private endpoints                 |
| DNS/private access | Private DNS zones, VNet links and name resolution after creating a private endpoint                                                             |
| Load balancing     | Layer 4 versus Layer 7 capabilities; health probes; inbound NAT rules; public versus internal load balancers                                    |
| Storage security   | SAS types, stored access-policy compatibility, access keys versus Entra authorization, firewall behaviour                                       |
| Storage resilience | LRS/ZRS/GRS/GZRS distinctions; whether failover and read access are available; replication boundaries                                           |
| Azure Files        | Identity-based authentication prerequisites, snapshots, soft delete and differences from Blob Storage                                           |
| Compute            | Availability sets versus zones; VM Scale Sets; disk types; VM resizing and move restrictions                                                    |
| Containers         | ACI versus Container Apps, registry authentication, revisions, ingress, scaling and environment boundaries                                      |
| App Service        | Plan versus app settings; scaling; deployment slots; slot-specific settings; custom domains and certificates                                    |
| ARM/Bicep          | Dependency and scope interpretation, parameter versus variable/output syntax, deployment mode and existing-resource references                  |
| Monitoring         | Activity Log versus resource logs versus metrics; diagnostic settings; Log Analytics; action groups and alert-processing rules                  |
| Backup/recovery    | Recovery Services vault versus Backup vault; soft delete; backup policies; restore operations; Site Recovery failover sequence                  |

- **Networking semantics**: You understand private endpoints, peering, NSGs and application connectivity professionally. The exam will ask narrow questions about effective routes, DNS linkage, non-transitive peering and exactly which resource must be modified.
- **Storage administration**: You use ADLS and managed identity, but AZ-104 goes sideways into Azure Files, stored access policies, SAS details, lifecycle rules, redundancy options and account-level settings.
- **Classic infrastructure**: VM availability sets, VMSS, managed disks, Recovery Services vaults and Site Recovery are less central to your Container Apps–led estate but remain heavily testable.
- **Licensing and SKU trivia**: Knowing the correct design does not necessarily tell you whether a feature requires Entra ID P1, a particular App Service tier or a particular storage configuration.
- **Portal terminology**: You may know what needs doing while not recognising Microsoft’s currently preferred blade, resource name or separation of responsibilities.
- **Choosing the minimum sufficient change**: Many questions ask what you should configure first, or which minimum set of actions meets the requirement. A technically valid but broader architecture is often the wrong answer.
