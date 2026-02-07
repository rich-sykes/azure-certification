# Microsoft Azure Fundamentals – 10-Day Certification Study Plans

This repository contains **structured, 10-day training plans** for Microsoft Azure **Fundamentals-level certifications**, designed for engineers and technical professionals who want to **pass efficiently without over-studying**.

Each certification plan is:
- Exam-aligned
- Time-boxed (10 days)
- Built around **high-signal video content**
- Optimised for people who already work with cloud, data, or AI systems

---

## 🎯 Certifications Covered

| Certification | Focus Area                      | Status     |
| ------------- | ------------------------------- | ---------- |
| **AZ-900**    | Azure Fundamentals              | ✅ Complete |
| **AI-900**    | Azure AI Fundamentals           | 🚧 Planned  |
| **DP-900**    | Azure Data Fundamentals         | 🚧 Planned  |
| **SC-900**    | Security, Compliance & Identity | ⏳ Future   |
| **PL-900**    | Power Platform Fundamentals     | ⏳ Future   |

---

## 🧠 Study Philosophy

These plans are designed for:
- Software engineers
- Data engineers / analysts
- Cloud engineers
- Architects
- Technical managers

### Principles
- **Clarity over depth** – fundamentals exams test concepts, not implementation
- **Video-first learning** – curated playlists with minimal redundancy
- **Exam-aware** – focus on how Microsoft frames questions
- **No busywork** – no labs unless they materially improve understanding

Each plan assumes:
- ⏱️ **60–75 mins/day on weekdays**
- ⏱️ **90 mins/day on weekends**
- 🧠 Existing technical literacy

---

## 📅 Structure of Each 10-Day Plan

Each certification folder contains:

- `README.md` – day-by-day study plan with:
  - Daily topics
  - Video links
  - Checklists
  - Key exam traps
- Optional:
  - Cram sheets
  - Practice questions
  - Final-day review guides

Example structure:

```
.
├── AZ-900/
│   └── README.md
├── AI-900/
│   └── README.md
├── DP-900/
│   └── README.md
└── README.md
```

---

## 📘 Current Plans

### ✅ AZ-900 – Azure Fundamentals
- Cloud concepts
- Azure architecture & services
- Identity, security & governance
- Cost management & SLAs

Uses:
- John Savill’s AZ-900 video series
- Official Microsoft instructor-led videos

➡️ See [`/AZ-900/README.md`](./AZ-900/README.md)

---

## 🧪 Exam Technique (Applies to All Plans)

Microsoft Fundamentals exams typically test:
- Definitions
- Use cases
- Service comparisons
- Responsibility boundaries

They **do not** test:
- Architecture depth
- Performance tuning
- Implementation detail

When unsure in an exam:
> Choose the **simplest**, **most managed**, **least administrative effort** option.

---

## 🚀 How to Use This Repo

1. Pick a certification
2. Follow the 10-day plan exactly
3. Tick off videos as you go
4. Do a practice exam on Day 9
5. Light review only on Day 10

This approach consistently yields **comfortable pass margins** without burnout.

---

## 🛠️ Contributions & Customisation

Feel free to:
- Fork the repo
- Adjust pacing
- Swap in alternative video sources
- Add personal notes or flashcards

This repo is intentionally **framework-first**, not prescriptive.

---

## 📌 Disclaimer

This repository is:
- Not affiliated with Microsoft
- Not a replacement for official documentation
- Designed to complement real-world experience

Certifications validate fundamentals — **experience builds mastery**.

---

## 📄 License

MIT License – use, adapt, and share freely.
# AZ-204 Readiness Checklist (Practical)

This checklist is for **exam alignment**, not learning Azure from scratch.

---

## 🧱 Develop Azure Compute Solutions (25–30%)

### Containerized solutions
- [ ] Build container images using Dockerfiles
- [ ] Tag images correctly (versioning vs `latest`)
- [ ] Push images to Azure Container Registry (ACR)
- [ ] Authenticate to ACR using Managed Identity
- [ ] Run containers using Azure Container Instances (ACI)
- [ ] Create and manage Azure Container Apps
- [ ] Know when to choose Container Apps vs ACI vs AKS

---

### Azure App Service Web Apps
- [ ] Create App Service (code-based)
- [ ] Create App Service (container-based)
- [ ] Configure application settings and environment variables
- [ ] Configure TLS / HTTPS
- [ ] Configure diagnostics and logging
- [ ] Deploy code and containerized apps
- [ ] Configure autoscaling rules
- [ ] Create and manage deployment slots
- [ ] Understand slot swap behavior (sticky vs non-sticky settings)

---

### Azure Functions
- [ ] Create and configure an Azure Functions app
- [ ] Choose hosting plan (Consumption vs Premium)
- [ ] Implement triggers:
  - [ ] HTTP
  - [ ] Timer
  - [ ] Storage / Queue
  - [ ] Webhooks
- [ ] Implement input and output bindings
- [ ] Explain why bindings are preferred over direct SDK usage
- [ ] Understand Durable Functions concepts:
  - [ ] Orchestrator
  - [ ] Activity
  - [ ] State management

---

## 💾 Develop for Azure Storage (15–20%)

### Azure Cosmos DB
- [ ] Perform CRUD operations using the SDK
- [ ] Understand containers vs items
- [ ] Choose the appropriate consistency level
- [ ] Explain consistency trade-offs
- [ ] Implement and explain the change feed
- [ ] Identify Cosmos DB use cases vs Azure SQL

---

### Azure Blob Storage
- [ ] Perform read/write operations using SDK
- [ ] Set and retrieve blob properties
- [ ] Set and retrieve blob metadata
- [ ] Understand blob access tiers (Hot, Cool, Archive)
- [ ] Implement lifecycle management policies
- [ ] Choose Blob vs File vs Queue storage correctly

---

## 🔐 Implement Azure Security (15–20%)

### Authentication and authorization
- [ ] Authenticate users using Microsoft Identity platform
- [ ] Authenticate apps using Microsoft Entra ID
- [ ] Understand delegated vs application permissions
- [ ] Implement RBAC for application access
- [ ] Create and use Shared Access Signatures (SAS)
- [ ] Know when NOT to use SAS

---

### Secure Azure solutions
- [ ] Store secrets in Azure Key Vault
- [ ] Access Key Vault using Managed Identity
- [ ] Use keys, secrets, and certificates securely
- [ ] Use Azure App Configuration for non-secret settings
- [ ] Explain why Managed Identity is preferred over secrets
- [ ] Interact with Microsoft Graph (conceptual understanding)

---

## 📊 Monitor and Troubleshoot Azure Solutions (5–10%)

- [ ] Instrument applications with Application Insights
- [ ] Monitor metrics, logs, and traces
- [ ] Understand requests vs dependencies vs exceptions
- [ ] Configure availability tests
- [ ] Configure alerts
- [ ] Use Live Metrics vs stored telemetry
- [ ] Diagnose performance issues using traces

---

## 🔗 Connect to Azure & Third-Party Services (20–25%)

### Azure API Management
- [ ] Create an API Management instance
- [ ] Create or import APIs
- [ ] Secure APIs using subscriptions or OAuth
- [ ] Configure rate limiting policies
- [ ] Apply transformation policies
- [ ] Understand APIM vs direct App Service exposure

---

### Event-based solutions
- [ ] Implement Azure Event Grid
- [ ] Identify event-driven use cases
- [ ] Implement Azure Event Hubs
- [ ] Identify streaming and telemetry use cases

---

### Message-based solutions
- [ ] Implement Azure Service Bus
- [ ] Understand queues vs topics
- [ ] Understand dead-letter queues
- [ ] Implement Azure Queue Storage
- [ ] Choose the correct messaging service:
  - [ ] Event Grid
  - [ ] Event Hubs
  - [ ] Service Bus
  - [ ] Queue Storage

---

## ✅ Final Readiness Check

You are ready for AZ-204 when you can:
- [ ] Explain *why* one service is chosen over another
- [ ] Default to Managed Identity for secure access
- [ ] Instantly distinguish messaging services
- [ ] Reason through scenario questions confidently
- [ ] Identify best-practice solutions, not just workable ones

---

**If most boxes are already checked, book the exam.**