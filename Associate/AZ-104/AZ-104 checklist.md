# AZ-104

## Skills at a glance

<https://learn.microsoft.com/en-gb/training/paths/az-104-administrator-prerequisites/>

- Manage Azure identities and governance (20–25%)
- Implement and manage storage (15–20%)
- Deploy and manage Azure compute resources (20–25%)
- Implement and manage virtual networking (15–20%)
- Monitor and maintain Azure resources (10–15%)

## 1. Manage Azure identities and governance (20–25%)

<https://learn.microsoft.com/en-gb/credentials/certifications/resources/study-guides/az-104#manage-azure-identities-and-governance-2025>

<https://learn.microsoft.com/en-gb/training/paths/az-104-manage-identities-governance/>

<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_01-Manage_Entra_ID_Identities.html>
<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_02a_Manage_Subscriptions_and_RBAC_Entra.html>
<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_02b-Manage_Governance_via_Azure_Policy.html>

### Manage Microsoft Entra users and groups

- Create users and groups
- [ ] **P2 — Dynamic groups**: Distinguish dynamic user and dynamic device groups; recognise the supported membership rules and that users and devices cannot be mixed in one dynamic group.
- [ ] **P2 — Dynamic membership licensing**: Know the Microsoft Entra licensing requirements for users benefiting from dynamic group membership.
- Manage user and group properties
- Manage licenses in Microsoft Entra ID
- Manage external users
- Configure self-service password reset (SSPR)

### Manage access to Azure resources

- Manage built-in Azure roles
- [ ] **P3 — Management plane versus data plane**: Distinguish control over the Azure resource from access to the data stored or processed by that resource, and select the appropriate RBAC role.
- [ ] **P2 — Managed identity types**: Compare system-assigned and user-assigned managed identities, including lifecycle, sharing, and role-assignment implications.
- Assign roles at different scopes
- [ ] **P3 — RBAC inheritance**: Role assignments inherit from parent scopes and are additive; a narrower assignment does not remove inherited permissions.
- Interpret access assignments

### Manage Azure subscriptions and governance

- Implement and manage Azure Policy
- [ ] **P1 — Modify effect versus tag inheritance**: Tags do not inherit automatically; use an Azure Policy `modify` effect to add or replace tags during resource creation or update.
- [ ] **P1 — Remediation of existing resources**: A policy assignment does not automatically change existing resources; create a remediation task for `modify` and `deployIfNotExists` policies.
- [ ] **P1 — Policy assignment identity and RBAC**: `modify` and `deployIfNotExists` remediation requires a managed identity on the assignment with the roles specified by the policy definition at the required scope.
- Configure resource locks
- [ ] **P3 — Locks versus Owner**: Resource locks apply regardless of Azure RBAC permissions; an Owner must remove the lock before performing a blocked management-plane operation.
- Apply and manage tags on resources
- Manage resource groups
- Manage subscriptions
- Manage costs by using alerts, budgets, and Azure Advisor recommendations
- Configure management groups

## 2. Implement and manage storage (15–20%)

<https://learn.microsoft.com/en-gb/credentials/certifications/resources/study-guides/az-104#implement-and-manage-storage-1520>

<https://learn.microsoft.com/en-gb/training/paths/az-104-manage-storage/>

<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_07-Manage_Azure_Storage.html>

### Configure and manage storage accounts

- [ ] Create and configure storage accounts
- [ ] Configure Azure Storage redundancy
- [ ] **P3 — Storage redundancy**: Compare LRS, ZRS, GRS, and RA-GRS by replication boundary, zone and region resilience, read access to the secondary, and failover behavior.
- [ ] Configure object replication
- [ ] Configure storage account encryption
- [ ] Manage data using Azure Storage Explorer
- [ ] Manage data using AzCopy

### Configure access to storage

- Configure Azure Storage firewalls and virtual networks
- Create and use shared access signature (SAS) tokens
- [ ] **P2 — SAS types**: Compare service SAS, account SAS, and user-delegation SAS by authorization source, supported services, resource scope, and permissions.
- Configure stored access policies
- [ ] **P2 — SAS revocation**: Use a stored access policy to change or revoke associated service SAS tokens before their individual expiry; know which SAS types support stored access policies.
- Manage access keys
- [ ] **P3 — Portal access**: Browsing storage data in the portal requires an appropriate data-plane role plus management-plane `Reader` access to navigate the storage account.
- Configure identity-based access for Azure Files
- [ ] **P3 — Azure Files SMB identity**: Understand the identity-source, domain-join, share-level RBAC, and file/directory permission requirements for identity-based SMB authentication.

### Configure Azure Files and Azure Blob Storage

- Create and configure a file share in Azure Files
- Create and configure a container in Azure Blob Storage
- Configure storage tiers
- Configure soft delete for blobs and containers
- Configure snapshots and soft delete for Azure Files
- Configure blob lifecycle management
- Configure blob versioning

## 3. Deploy and manage Azure compute resources (20–25%)

<https://learn.microsoft.com/en-gb/credentials/certifications/resources/study-guides/az-104#deploy-and-manage-azure-compute-resources-2025>

<https://learn.microsoft.com/en-gb/training/paths/az-104-manage-compute-resources/>

<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_03b-Manage_Azure_Resources_by_Using_ARM_Templates.html>
<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_08-Manage_Virtual_Machines.html>
<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_09a-Implement_Web_Apps.html>
<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_09b-Implement_Azure_Container_Instances.html>
<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_09c-Implement-Azure-Container-Apps.html>

### Automate deployment of resources by using Azure Resource Manager (ARM) templates or Bicep files

- Interpret an Azure Resource Manager template or a Bicep file
- [ ] **P3 — Deployment modes**: Incremental mode leaves resources not declared in the template unchanged; complete mode deletes resources in the target resource group that are not declared, subject to documented exceptions.
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
- [ ] **P2 — Managed-disk expansion**: Expand the Azure managed disk first, then extend the partition and filesystem inside the guest OS; understand when deallocation is required.
- Deploy virtual machines to availability zones and availability sets
- [ ] **P1 — Availability zones versus sets**: Zones distribute VMs across separate datacentres in a region; availability sets distribute VMs across fault and update domains within a datacentre grouping. Know their deployment constraints and SLA implications.
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
- [ ] **P2 — Slot settings and stickiness**: Distinguish settings that swap from deployment-slot settings that remain with a slot; configure sticky app settings and connection strings and understand swap behavior.

## 4. Implement and manage virtual networking (15–20%)

<https://learn.microsoft.com/en-gb/credentials/certifications/resources/study-guides/az-104#implement-and-manage-virtual-networking-1520>

<https://learn.microsoft.com/en-gb/training/paths/az-104-manage-virtual-networks/>

<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_04-Implement_Virtual_Networking.html>
<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_05-Implement_Intersite_Connectivity.html>
<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_06-Implement_Network_Traffic_Management.html>

### Configure and manage virtual networks in Azure

- Create and configure virtual networks and subnets
- Create and configure virtual network peering
- [ ] **P3 — Peering topology**: VNet peering is non-transitive; each required VNet-to-VNet connection needs direct peering or a supported hub-routing design.
- Configure public IP addresses
- Configure user-defined routes
- [ ] **P1 — Longest-prefix route selection**: Azure first selects the matching route with the longest prefix, regardless of whether its source is system, BGP, or user-defined.
- [ ] **P1 — Equal-prefix source priority**: When matching prefix lengths are equal, Azure generally prefers a user-defined route, then a BGP route, then a system route.
- [ ] **P2 — UDRs and virtual appliances**: Route traffic to a virtual appliance with the correct next-hop IP; enable IP forwarding on its NIC and within the appliance operating system.
- Troubleshoot network connectivity

###  Configure secure access to virtual networks

- Create and configure network security groups (NSGs) and application security groups
- [ ] **P2 — Subnet and NIC NSG evaluation**: For inbound traffic Azure evaluates the subnet NSG before the NIC NSG; for outbound traffic it evaluates the NIC NSG before the subnet NSG.
- [ ] **P3 — NSGs at every layer**: Traffic must be permitted by every applicable NSG; an allow rule at one layer cannot override a deny at another.
- Evaluate effective security rules in NSGs
- Implement Azure Bastion
- Configure service endpoints for Azure platform as a service (PaaS)
- Configure private endpoints for Azure PaaS
- [ ] **P1 — Private versus service endpoints**: A private endpoint gives a service a private IP in the VNet; a service endpoint keeps the service's public endpoint while extending the subnet identity over the Azure backbone.
- [ ] **P1 — Private DNS zones and VNet links**: Configure the service-specific `privatelink` zone, link every VNet that must resolve it, and understand the role of private DNS zone groups.
- [ ] **P1 — Storage private-endpoint DNS path**: Trace the storage account public name through its `privatelink` CNAME to the private DNS A record and private IP; account for custom DNS forwarding when clients do not use Azure-provided DNS directly.

### Configure name resolution and load balancing

- Configure Azure DNS
- Configure an internal or public load balancer
- Troubleshoot load balancing

## 5. Monitor and maintain Azure resources (10–15%)

<https://learn.microsoft.com/en-gb/credentials/certifications/resources/study-guides/az-104#monitor-and-maintain-azure-resources-1015>

<https://learn.microsoft.com/en-gb/training/paths/az-104-monitor-backup-resources/>

<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_10-Implement_Data_Protection.html>
<https://microsoftlearning.github.io/AZ-104-MicrosoftAzureAdministrator/Instructions/Labs/LAB_11-Implement_Monitoring.html>

### Monitor resources in Azure

- Interpret metrics in Azure Monitor
- Configure log settings in Azure Monitor
- Query and analyze logs in Azure Monitor
- Set up alert rules, action groups, and alert processing rules in Azure Monitor
- [ ] **P3 — Scheduled notification suppression**: Use an alert processing rule with a schedule to suppress or reroute notifications without disabling the underlying alert rules.
- Configure and interpret monitoring of virtual machines, storage accounts, and networks by using Azure Monitor Insights
- Use Azure Network Watcher and Connection monitor

### Implement backup and recovery

- Create a Recovery Services vault
- Create an Azure Backup vault
- [ ] **P2 — Recovery Services vault versus Backup vault**: Choose the vault type supported by the datasource and scenario; recognise that the two vault resources are not interchangeable.
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
