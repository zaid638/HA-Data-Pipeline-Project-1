# HA-Data-Pipeline-Project-1<br/>

## 📌 Project Overview<br/>

This project implements an **automated cross-cloud data pipeline to restore SQL Server databases using backup files transferred from Azure to Google Cloud Platform (GCP)**. The pipeline ensures **reliable data movement**, **restoration**, **logging**, and **alerting** to support operational database recovery workflows.

The solution is designed with **fault tolerance**, **observability**, and **automation** in mind, making it suitable for enterprise-scale database restoration and migration use cases.<br/><br/>


## 🏗️ Architecture Overview<br/>

!(Pipline Architecture)[https://github.com/zaid638/HA-Data-Pipeline-Project-1/blob/main/datapipeline_architecture_2.drawio.png]<br/>

The pipeline consists of the following major components:
1. Azure – Source environment where SQL Server backup files originate.
2. Google Cloud Platform (GCP) – Intermediate cloud used for storage, orchestration, and processing.
3. Database Restoration Files – Backup files staged for SQL Server restoration.
4. SQL Server – Target database server where restoration is performed.
5. Logging System – Captures operational logs at multiple pipeline stages.
6. Email Alerting – Notifies stakeholders in case of failures or critical events.<br/><br/>

## 🔄 Data Flow<br/>

1. Backup files are transferred from Azure to GCP.
2. GCP processes and stores the database restoration files.
3. Restoration files are used to restore the database on SQL Server.
4. Log data is generated during:
	- Cloud transfer and processing (GCP)
	- Database restoration phase
5. Email alerts are triggered for:
	- Pipeline failures
	- Restoration errors<br/><br/>

## ⚙️ Key Features<br/>

✅ Cross-cloud data movement (Azure → GCP)
✅ Automated SQL Server database restoration
✅ Centralized logging for observability
✅ Email-based alerting for failures
✅ Modular and scalable architecture
✅ Production-ready pipeline design<br/><br/>

## 🚨 Error Handling & Monitoring<br/>

- All critical steps generate logs.
- Failures trigger automated email alerts.
- Logs can be used for root-cause analysis and auditing.<br/><br/>

