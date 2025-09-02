# Car Sales Data Engineering Project with Azure

This project demonstrates an **end-to-end Azure Data Engineering pipeline** that ingests car sales data, processes it through the **Medallion Architecture (Bronze → Silver → Gold)**, and delivers analytics-ready data in a **star schema model**.

---

##  Project Overview

- **Source**: Raw car sales data hosted on GitHub  
- **Ingestion**: Data moved from GitHub → Azure SQL Database using **Azure Data Factory**  
- **Bronze Layer**: Raw data stored in Azure Data Lake  
- **Silver Layer**: Data cleaned and transformed (e.g., derived columns for insights like revenue per unit etc.)  
- **Gold Layer**: Data modeled into a **Star Schema** with Fact (sales transactions) and Dimension (model, dealers, date, branch) tables  

---

## Project Architecture

**High-level pipeline flow**  
  ![Project Architecture](https://github.com/pabodaR/Sales-Azure-Data-Engineering-Project/blob/main/architecture.jpg?raw=true)

---

## Medallion Architecture

- **Bronze** → Raw ingestion (unaltered source data)  
- **Silver** → Cleaned + enriched data (added calculated columns for deeper insights)  
- **Gold** → Star schema (Fact + Dim tables for reporting and BI consumption)  

![Medallion Architecture](https://github.com/pabodaR/Sales-Azure-Data-Engineering-Project/blob/main/Medallion.jpg?raw=true)

---

## Problem Solved

Raw car sales data was scattered and unstructured, making reporting inefficient.  
This project provides:  
- A **scalable, dynamic pipeline** for ingestion and processing  
- A **clean, structured dataset** ready for analytics  
- A **star schema** that enables fast querying and BI integration  

---

## Tech Stack

- **Azure Data Factory** (data movement & orchestration)  
- **Azure SQL Database** (staging & transformation)  
- **Azure Data Lake Storage** (Bronze, Silver, Gold layers)
- **Azure DataBricks** (Data Transformations and Preprocessing)  
- **Star Schema Modeling** (Fact & Dimension tables)  

---

## Star Schema

- Fact table: `FactSales`  
- Dimensions: `DimDate`, `DimBranch`, `DimDealer`, `DimModel`  

![Star Schema](https://github.com/pabodaR/Sales-Azure-Data-Engineering-Project/blob/main/Star.jpg?raw=true)


---


