# Database-Migration-from-On-Premise-to-Google-Cloud-SQL

This project demonstrates how to migrate an existing **MySQL database** from an on-premise virtual machine to **Google Cloud SQL** using **Google Cloud Database Migration Service (DMS)**.  
The goal was to enable secure, continuous synchronization with minimal downtime and ensure zero data loss.

---

##  Project Overview
- Source: On-premise VM running MySQL 8.0.41  
- Target: Google Cloud SQL (MySQL)  
- Migration Tool: Google Cloud Database Migration Service (DMS) with **Change Data Capture (CDC)**  
- Connectivity: Secure **VPC Peering** between source and GCP  
- Monitoring: Google Cloud Console for migration jobs and sync status  

---

##  Contributions
- Set up the MySQL database on the virtual machine.  
- Configured and ran the Database Migration Service (DMS).  
- Verified data migration and live synchronization.  
- Automated the migration process using cron jobs.  
- Configured the Cloud SQL instance on GCP and worked on VPC peering for secure connection.  
- Assisted in migration testing and troubleshooting.  
- Configured the Migration Connection Profile for the source VM and created the Migration Job for seamless integration between source and destination.  
- Created dummy data, verified migration on the destination VM, and resolved firewall/network settings issues.  

---

##  Technology Used
- **Google Cloud SQL** – Managed MySQL database service  
- **Google Cloud Database Migration Service (DMS)**  
- **MySQL v8.0.41** on Virtual Machine  
- **VPC Peering** for secure connectivity  
- **Google Cloud Console** for job setup and monitoring  

---

##  Features Implemented
- Continuous Data Sync with CDC (Change Data Capture)  
- Secure VPC Peering between source VM and GCP  
- Minimal Downtime Migration  
- Live Data Monitoring and Validation  
- Automated Migration Job  

---

##  Architecture
**Source:** On-premise VM (MySQL 8.0.41)  
**Target:** Google Cloud SQL (MySQL)  
**Connection:** Remote-access user + VPC Peering  
**Tool:** Google Cloud DMS (CDC enabled)  

![image alt](https://github.com/Abhishekg07/Database-Migration-from-On-Premise-to-Google-Cloud-SQL/blob/1de822201d5eab8919c06a0843e2906bf9a33366/Architecture%20Diagram.png)

---

##  Challenges & Solutions
- **Network/Firewall Restrictions:** Opened required ports and verified with MySQL clients.  
- **Schema Mismatches:** Validated and aligned schemas before migration.  
- **Connection Timeouts:** Used VPC Peering for stable connectivity.  
- **Continuous Sync Issues:** Verified CDC with manual inserts and GCP Console monitoring.  

---

##  Final Outcome
- Successfully migrated the MySQL database to **Google Cloud SQL**.  
- Achieved **live synchronization with zero data loss**.  
- Real-time updates reflected in Cloud SQL.  
- Reduced administrative overhead using a cloud-native managed database.  

---

##  Future Improvements
- Add automated post-migration data validation and alerts.  
- Expand support for multiple schema migrations.  
- Integrate **BigQuery** for advanced analytics.  
- Automate rollback/recovery in case of sync failure.  

---

##  Project Info
This project was completed as part of coursework at **Binghamton University (SUNY)**.  
It demonstrates how cloud-native tools like **Google Cloud SQL** and **DMS** simplify complex data migrations, ensuring performance, scalability, and security.  
