# DP-900 – Skills at a Glance (Exam Checklist + Best Videos)

Use this as a **progress tracker** and **final readiness checklist** before exam day.

Reddit consensus:
- Microsoft Learn = foundation
- John Savill = framing + exam mindset
- A small number of targeted explainers for concepts

---

## 🧱 Describe Core Data Concepts (25–30%)

### Ways to Represent Data
- [ ] Structured data  
  ▶️ John Savill – Data fundamentals overview  
  https://youtu.be/8Y3H0J9Y0yw

  - [ ] Tabular format (rows & columns)
  - [ ] Fixed schema

- [ ] Semi-structured data  
  ▶️ Microsoft – Structured vs semi-structured vs unstructured  
  https://youtu.be/bAyrObl7TYE

  - [ ] Flexible schema
  - [ ] JSON / XML examples

- [ ] Unstructured data  
  ▶️ Same video as above (conceptual grouping)

  - [ ] No predefined schema
  - [ ] Text, images, video

---

### Options for Data Storage
- [ ] Common data file formats  
  ▶️ John Savill – Data formats explained  
  https://youtu.be/2wVdK2xS1BQ

  - [ ] CSV
  - [ ] JSON
  - [ ] XML
  - [ ] Parquet (columnar)

- [ ] Types of databases  
  ▶️ Microsoft – Relational vs non-relational databases  
  https://youtu.be/ztHopE5Wnpc

  - [ ] Relational databases
  - [ ] Non-relational (NoSQL) databases

---

### Common Data Workloads
- [ ] Transactional workloads (OLTP)  
- [ ] Analytical workloads (OLAP)  

▶️ John Savill – OLTP vs OLAP (DP-900 focus)  
https://youtu.be/vbHqUNl8YFk

  - [ ] High volume of small reads/writes
  - [ ] Large-scale reads & aggregations

---

### Roles and Responsibilities
- [ ] Database administrator (DBA)
- [ ] Data engineer
- [ ] Data analyst

▶️ Microsoft – Data roles explained  
https://youtu.be/f4Yc6Z9t8QY

---

## 🗄️ Identify Considerations for Relational Data on Azure (20–25%)

### Relational Data Concepts
- [ ] Features of relational data
- [ ] Normalization
- [ ] Common SQL statements
- [ ] Common database objects

▶️ John Savill – Relational data fundamentals  
https://youtu.be/MGZbQpVvPpA

---

### Relational Azure Data Services
- [ ] Azure SQL Database
- [ ] Azure SQL Managed Instance
- [ ] SQL Server on Azure Virtual Machines

▶️ Microsoft – Azure SQL options compared  
https://youtu.be/kc0zC2fXwG8

(Reddit tip: **focus on when to choose which**, not feature lists)

---

### Open-source Database Services on Azure
- [ ] Azure Database for MySQL
- [ ] Azure Database for PostgreSQL
- [ ] Azure Database for MariaDB

▶️ Microsoft – Open-source databases on Azure  
https://youtu.be/XyFz5WcF7bQ

---

## 📦 Describe Considerations for Non-Relational Data on Azure (15–20%)

### Azure Storage Capabilities
- [ ] Azure Blob Storage
- [ ] Azure File Storage
- [ ] Azure Table Storage

▶️ John Savill – Azure Storage explained  
https://youtu.be/SY1p6pJp3fQ

---

### Azure Cosmos DB
- [ ] Core capabilities
- [ ] Use cases
- [ ] APIs

▶️ John Savill – Azure Cosmos DB fundamentals  
https://youtu.be/1BfCnj0PjZg

(Reddit note: **Cosmos DB comes up a lot** — understand *why* you’d use it)

---

## 📊 Describe an Analytics Workload (25–30%)

### Large-Scale Analytics Concepts
- [ ] Ingest
- [ ] Store
- [ ] Process
- [ ] Visualize

▶️ Microsoft – Analytics workloads explained  
https://youtu.be/6bqZJ4K4mFg

---

### Analytical Data Stores
- [ ] Data warehouses
- [ ] Data lakes
- [ ] Lakehouse concept

▶️ John Savill – Data warehouse vs data lake  
https://youtu.be/dV7uR4mCz3U

---

### Azure Analytics Services
- [ ] Azure Databricks
- [ ] Microsoft Fabric

▶️ Microsoft – Azure analytics services overview  
https://youtu.be/JBqFh4jYp4A

(Reddit consensus: **don’t go deep, know what problem each solves**)

---

### Real-Time Analytics
- [ ] Batch processing
- [ ] Streaming processing
- [ ] Batch vs streaming differences
- [ ] Real-time analytics use cases

▶️ Microsoft – Batch vs streaming analytics  
https://youtu.be/4l0n6mQ2Yk8

---

### Data Visualization with Power BI
- [ ] Power BI capabilities
- [ ] Data models in Power BI

▶️ Microsoft – Power BI fundamentals for DP-900  
https://youtu.be/TmhQCQr_DCA

---

## ✅ Exam Readiness Rule

You are **DP-900 ready** when:
- [ ] You can explain each checked item in **one sentence**
- [ ] You can choose **relational vs non-relational** from a scenario
- [ ] You can choose **transactional vs analytical** workloads
- [ ] You can identify the **correct Azure service** for each workload

---

## Final Reddit Advice (Worth Remembering)

- Don’t memorise SKUs or pricing  
- Think in **use cases**
- Choose **managed services first**
- If two answers look right, pick the **simpler Azure-native one**