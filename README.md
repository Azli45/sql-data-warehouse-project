# 🏛️ SQL Data Warehouse Project

> A fully implemented modern data warehouse built on SQL Server — integrating dual source systems through a Medallion Architecture and delivering SQL-based analytics across sales, customers, and products.

![SQL](https://img.shields.io/badge/SQL-T--SQL-CC2927?logo=microsoftsqlserver&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-Data%20Warehouse-003B5C?logo=microsoftsqlserver&logoColor=white)
![Architecture](https://img.shields.io/badge/Architecture-Medallion-gold)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Overview

An end-to-end data warehousing solution that consolidates data from two source systems — **ERP** and **CRM** — into a single, analytics-ready warehouse on SQL Server. The project covers the full data engineering lifecycle: ingestion, cleansing, integration, modelling, and reporting.

Built to mirror real industry workflows, with a clean **Bronze → Silver → Gold** medallion architecture and a star schema Gold layer optimized for analytical queries.

---

## 🏗️ Data Architecture

```
┌─────────────┐     ┌─────────────┐
│  ERP (CSV)  │     │  CRM (CSV)  │
└──────┬──────┘     └──────┬──────┘
       └─────────┬──────────┘
                 ▼
        🥉 Bronze Layer
        Raw ingestion — no transformation
                 ▼
        🥈 Silver Layer
        Cleansing · Standardization · Normalization
                 ▼
        🥇 Gold Layer
        Star Schema — Fact & Dimension Tables
                 ▼
        📊 SQL Analytics & Reporting
```

| Layer | Role |
|-------|------|
| 🥉 **Bronze** | Raw CSV data loaded as-is into SQL Server — full fidelity source preservation |
| 🥈 **Silver** | Data quality fixes, type normalization, deduplication, and standardization |
| 🥇 **Gold** | Business-ready star schema powering all analytical queries |

---

## ✅ What's Built

### 🔄 ETL Pipeline
- Ingestion from two independent source systems (ERP + CRM CSV files)
- Data quality resolution: nulls, type mismatches, duplicates, inconsistent codes
- Integration of both sources into a unified, conformed data model

### 🗃️ Data Modelling — Star Schema
- **Fact Table** — transactional sales records
- **Dimension Tables** — customers, products, and supporting attributes
- Optimized for fast analytical queries and BI consumption

### 📊 SQL Analytics & Reporting
Three analytical domains fully implemented:

| Domain | Insights Delivered |
|--------|-------------------|
| 👤 **Customer Behavior** | Purchase frequency, customer segmentation, lifetime value patterns |
| 📦 **Product Performance** | Top/bottom performers, category contribution, sales volume trends |
| 📈 **Sales Trends** | Period-over-period growth, revenue patterns, time-based aggregations |



---

## 🛠️ Tech Stack

| Category | Tool |
|----------|------|
| Query Language | T-SQL (Transact-SQL) |
| Database Engine | Microsoft SQL Server |
| Architecture Pattern | Medallion (Bronze / Silver / Gold) |
| Data Modelling | Star Schema (Fact + Dimensions) |
| IDE | SSMS / Azure Data Studio |

---

## 🎯 Business Value

This warehouse enables stakeholders to:
- Query **clean, integrated data** from two previously siloed systems
- Analyse **sales trends, customer segments, and product performance** without touching raw data
- Trust results backed by **automated quality tests** across every pipeline layer

---

## 👤 Author

**Azli Khan**
Aspiring Data Engineer | SQL · Data Warehousing · ETL · Analytics

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?logo=linkedin)](https://www.linkedin.com/in/azli-khan07/)
[![GitHub](https://img.shields.io/badge/GitHub-Azli45-181717?logo=github)](https://github.com/Azli45)

---

## 📄 License

Licensed under the [MIT License](LICENSE).

---

> ⭐ Found this useful? Give it a star!
