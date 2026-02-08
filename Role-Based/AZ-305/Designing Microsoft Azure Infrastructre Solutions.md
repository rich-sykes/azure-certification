# AZ-305 – Designing Microsoft Azure Infrastructure Solutions
_Source: Microsoft Learn Study Guide_

---

## 1. Design identity, governance, and monitoring solutions (≈25%)

### Identity & Access
- [ ] Understand Microsoft Entra ID vs on-prem AD
- [ ] Users vs service principals vs managed identities
- [ ] System-assigned vs user-assigned managed identities
- [ ] Authentication vs authorization
- [ ] Azure RBAC vs custom roles
- [ ] Built-in roles vs least-privilege design

### Governance
- [ ] Management groups hierarchy and use cases
- [ ] Subscription design (prod / non-prod separation)
- [ ] Resource groups vs subscriptions (scope decisions)
- [ ] Azure Policy vs RBAC (when to use which)
- [ ] Policy initiatives (policy sets)
- [ ] Tagging strategies for cost & ownership
- [ ] Blueprint concept (high-level understanding)

### Monitoring & Observability
- [ ] Azure Monitor vs Log Analytics vs App Insights
- [ ] Centralised logging across subscriptions
- [ ] Metrics vs logs vs traces
- [ ] Alerts (metric vs log-based)
- [ ] Diagnostic settings
- [ ] Designing for operational visibility

---

## 2. Design data storage solutions (≈25%)

### Relational Data
- [ ] Azure SQL Database vs Managed Instance vs SQL on VM
- [ ] Single DB vs elastic pools
- [ ] Read scale-out options
- [ ] Geo-replication & failover groups
- [ ] Backup retention options
- [ ] RPO vs RTO trade-offs for SQL

### Non-Relational Data
- [ ] Azure Cosmos DB use cases
- [ ] Core (SQL) API vs MongoDB API
- [ ] Consistency levels (strong → eventual)
- [ ] Throughput models (manual vs autoscale)
- [ ] Multi-region reads/writes

### Storage Accounts
- [ ] Blob vs File vs Queue vs Table storage
- [ ] Hot / Cool / Archive tiers
- [ ] Data Lake Storage Gen2 use cases
- [ ] Lifecycle management rules
- [ ] Secure access (private endpoints, SAS)

### Backup & Recovery
- [ ] Azure Backup vs native service backups
- [ ] When to use snapshots vs backups
- [ ] Geo-redundant vs locally redundant storage

---

## 3. Design business continuity solutions (≈15%)

### High Availability
- [ ] Availability sets vs availability zones
- [ ] Zone-redundant vs zone-pinned services
- [ ] Stateless vs stateful design implications
- [ ] SLA composition (why 99.99% matters)

### Disaster Recovery
- [ ] Active/active vs active/passive
- [ ] Regional pairing concepts
- [ ] Backup vs replication vs DR
- [ ] Traffic Manager vs Azure Front Door
- [ ] Designing to meet RPO/RTO requirements

### Failure Scenarios
- [ ] Planned vs unplanned outages
- [ ] Single-region vs multi-region designs
- [ ] Cost vs resilience trade-offs

---

## 4. Design infrastructure solutions (≈35%)

### Compute
- [ ] App Service vs Azure Functions
- [ ] Container Apps vs AKS vs VMs
- [ ] Stateless application design
- [ ] Autoscaling strategies
- [ ] Background processing patterns

### Networking
- [ ] VNet basics and CIDR planning
- [ ] Hub-and-spoke topology
- [ ] Peering vs VPN vs ExpressRoute
- [ ] Private endpoints vs service endpoints
- [ ] NSGs vs Azure Firewall vs WAF
- [ ] Application Gateway vs Front Door

### Integration & Messaging
- [ ] Event Grid vs Event Hubs vs Service Bus
- [ ] Event-driven vs message-based systems
- [ ] Synchronous vs asynchronous design

### Security by Design
- [ ] Network isolation strategies
- [ ] Zero Trust principles
- [ ] Secure service-to-service communication
- [ ] Secrets management (Key Vault)

---

## Exam Readiness Checklist

- [ ] Can explain *why* one service is chosen over another
- [ ] Comfortable with ambiguous scenarios
- [ ] Can eliminate options that violate constraints
- [ ] Thinks in managed services first
- [ ] Considers cost, ops, and governance in every answer
- [ ] Confident with case study question format

---

## Final Reminder
AZ-305 is not about configuration steps.
It is about **making defensible architectural decisions under constraints**.