# 🚗 **Car Enterprise Project – End-to-End Data Engineering Pipeline** 🚗

An end-to-end modern data engineering project built on Microsoft Azure, using real-world car sales data as the source.

This project follows the **Medallion Architecture** (Bronze → Silver → Gold) and demonstrates ingestion, transformation, and reporting using Azure-native tools.

---

## ❓ **Problem**

Organizations often face challenges with:
- Ingesting raw data from external sources
- Transforming large and messy datasets
- Structuring data for easy analysis
- Ensuring secure access between services
- Creating reliable dashboards for reporting

---

## ✅ **Solution**

This project solves these challenges by:
- 🚀 **Ingestion**: Using **Azure Data Factory** to dynamically pull car sales data into the **Bronze** layer.
- ⚙️ **Transformation**: Leveraging **Azure Databricks** and **PySpark** to clean, transform, and enrich the data in the **Silver** layer.
- 🧠 **Storage**: Storing cleaned and structured data in **Delta Lake** format in the **Gold** layer for analytics and querying.
- 🔐 **Security**: Securing access to the data pipeline using **Microsoft Entra ID** and **OAuth** for authentication.
- 📊 **Visualization**: Connecting **Power BI** to the Gold Layer data in Databricks to create interactive dashboards.

---

## 🏗️ **Architecture Overview**

![Azure Car Enterprise Project Architecture](https://raw.githubusercontent.com/girald02/Azure-Car-Enterprise-Project-3/refs/heads/main/img/linkedin/1.png)

---

## 📊 **Data Source**

- **Car Sales Data**: The source data represents car sales records, including various attributes such as make, model, year, and price.  
  (You can replace this with your actual dataset info if needed!)

---

## 🧩 **Tech Stack**

| Tool                     | Purpose                                    |
|--------------------------|--------------------------------------------|
| **Azure Data Factory**    | Ingest raw files from Azure SQL Database dynamically     |
| **Azure Data Lake Gen2**  | Store raw data in **Bronze** and transformed data in **Silver** and **Gold** layers     |
| **Azure Databricks**      | Transform and clean data using **PySpark**               |
| **Delta Lake**            | Enable versioning and time-travel for clean data storage    |
| **Power BI**              | Visualize and create dashboards from final data                   |
| **Microsoft Entra ID (AAD)** | Secure access control and authentication via OAuth             |

---

## ✅ **Project Phases**

### 🚀 **Phase 1: Ingestion with Azure Data Factory (Bronze Layer)**

- Built dynamic **Azure Data Factory** pipelines to pull car sales data from a SQL Database into the **Bronze** layer.
- Used **parameterized pipelines** for flexibility and scalability.
- Stored raw data in **Parquet** format in Azure Data Lake Gen2.

---

### ⚙️ **Phase 2: Transformation with Azure Databricks (Silver Layer)**

- Connected **Azure Databricks** securely to Azure Data Lake using **App Registration** for access control.
- Cleaned and enriched the raw car sales data using **PySpark** scripts in Databricks notebooks.
- Stored the cleaned data in the **Silver** layer for further analysis.

---

### ⚙️ **Phase 3: Delta Lake – Gold Layer**

- Converted the cleaned data into **Delta Lake** format, providing features like **schema enforcement** and **versioning**.
- Enabled **Time Travel** capabilities to track historical changes in the data.
- Stored the final clean data in the **Gold** layer for business intelligence use.

---

### 📊 **Phase 4: Business Intelligence with Power BI**

- Integrated **Power BI** with **Databricks** using Azure Marketplace connectors.
- Generated an access token via **Databricks Developer Settings** for secure access.
- Created **Power BI** dashboards to visualize key car sales metrics like price trends, sales by model, and regional sales performance.

---

## 🔐 **Security & Access Control**

- Secured access between **Azure Data Factory**, **Databricks**, and **Azure Data Lake** using **Microsoft Entra ID** (Azure Active Directory).
- Registered an **Application (App Registration)** for Databricks to access the data lake.
- Used **OAuth authentication** to ensure secure interactions between the services.
- Applied **role-based access control** (RBAC) through Azure IAM to assign appropriate permissions (e.g., **Storage Blob Data Contributor**).

---

## 🙌 **Acknowledgments**

> 🎓 **Special thanks to [Ansh Lamba](https://github.com/anshlambagit)** for the incredible tutorial that inspired and guided this project. His teachings are a great resource for anyone learning **Azure Data Engineering**!

---

## 📌 **Key Features Implemented**

- ✅ Parameterized pipeline ingestion in **Azure Data Factory**  
- ✅ Scalable data architecture using **Medallion Architecture** (Bronze, Silver, Gold layers)  
- ✅ Data transformations using **PySpark** in **Azure Databricks**  
- ✅ **Delta Lake** storage with versioning & time travel for data management  
- ✅ Secure **OAuth** authentication via **Microsoft Entra ID**  
- ✅ Interactive dashboards created using **Power BI** for data insights  

---

## 📎 **Useful Links**

- [GitHub Repository](https://github.com/girald02/Azure-Car-Enterprise-Project-3)  
- [Ansh Lamba's Tutorial](https://www.youtube.com/watch?v=6_hXeNg9TJ0)  

---

## 🤝 **Let’s Connect!**

I’m always open to feedback, collaboration, or discussing **Azure Data Engineering**.  
Feel free to **open issues** or connect with me on [LinkedIn](https://www.linkedin.com/in/girald-bacongan-988144174/).
