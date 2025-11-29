# Business Intelligence System: Sales Performance Analysis

## 📊 Project Overview
This project implements a comprehensive Business Intelligence (BI) system for analyzing sales performance using MySQL database as the foundation. The solution includes data warehouse design, ETL processes, and interactive dashboard development.

## 🎯 Project Objectives
- Design and implement a sales-focused data mart
- Develop automated ETL pipelines for data integration
- Create interactive dashboards with key performance indicators
- Establish a complete BI infrastructure from operational data

## 🏗️ System Architecture
The solution follows a layered architecture:

1. **Data Source Layer**: MySQL operational database ("comptoir")
2. **ETL Layer**: Talend Open Studio for data extraction and transformation
3. **Data Warehouse Layer**: MySQL-based data mart with star schema
4. **Presentation Layer**: Power BI for visualization and analytics

## 📁 Project Structure
<img width="519" height="463" alt="image" src="https://github.com/user-attachments/assets/06ff0e8e-32b5-4919-98c3-aa90281a5810" />

## 🛠️ Technology Stack
- **Database Management**: MySQL 8.0+
- **Data Modeling**: MySQL Workbench
- **ETL Tool**: Talend Open Studio for Data Integration
- **BI & Visualization**: Microsoft Power BI
- **Version Control**: Git/GitHub

## 📋 Deliverables

### Deliverable 1: Technical Design Document
- Business requirements and KPIs identification
- Star schema design with fact and dimension tables
- Dimension hierarchies definition
- Technology comparison and justification
- Architecture blueprint

### Deliverable 2: Data Warehouse Implementation
- Complete SQL script for data mart creation (`comptoirED.sql`)
- User access configuration (analyst role with restricted privileges)
- Database schema validation

### Deliverable 3: ETL Solution
- Talend Open Studio project export
- Data extraction and transformation jobs
- Incremental loading strategies
- Data quality checks

### Deliverable 4: Analytics Dashboard
- Power BI project file with interactive visualizations
- Sales performance KPIs and metrics
- Drill-down capabilities and filters
- Executive summary views

## 🔐 Security Configuration
```sql
-- Root user configuration
ALTER USER 'root'@'localhost' IDENTIFIED BY '1234@Bi';

-- Analyst user creation
CREATE USER 'analyste'@'localhost' IDENTIFIED BY 'ED1234@';
GRANT ALL PRIVILEGES ON comptoirED.* TO 'analyste'@'localhost';
