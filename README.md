# 🚗 Car Sales Data Engineering Project with Azure

This project demonstrates an **end-to-end Azure Data Engineering pipeline** that ingests car sales data, processes it through the **Medallion Architecture (Bronze → Silver → Gold)**, and delivers analytics-ready data in a **star schema model**.

---

## 📌 Project Overview

- **Source**: Raw car sales data hosted on GitHub  
- **Ingestion**: Data moved from GitHub → Azure SQL Database using **Azure Data Factory**  
- **Bronze Layer**: Raw data stored in Azure Data Lake  
- **Silver Layer**: Data cleaned and transformed (e.g., derived columns for insights like revenue per unit etc.)  
- **Gold Layer**: Data modeled into a **Star Schema** with Fact (sales transactions) and Dimension (model, dealers, date, branch) tables  

---

## 🛠️ Architecture

**High-level pipeline flow**  
📍 *[Insert Architecture Diagram Here]*

---

## 🗂️ Medallion Architecture

- **Bronze** → Raw ingestion (unaltered source data)  
- **Silver** → Cleaned + enriched data (added calculated columns for deeper insights)  
- **Gold** → Star schema (Fact + Dim tables for reporting and BI consumption)  

📍 *[Insert Medallion Architecture Diagram Here]*

---

## 💡 Problem Solved

Raw car sales data was scattered and unstructured, making reporting inefficient.  
This project provides:  
- A **scalable, automated pipeline** for ingestion and processing  
- A **clean, structured dataset** ready for analytics  
- A **star schema** that enables fast querying and BI integration  

---

## 🚀 Tech Stack

- **Azure Data Factory** (data movement & orchestration)  
- **Azure SQL Database** (staging & transformation)  
- **Azure Data Lake Storage** (Bronze, Silver, Gold layers)  
- **Star Schema Modeling** (Fact & Dimension tables)  

---

## 📊 Example Outputs

- Fact table: `FactSales`  
- Dimensions: `DimDate`, `DimBranch`, `DimDealer`, `DimModel`  

📍 *[Insert Sample Schema Diagram Here]*

---

## 📂 Repo Structure

