# Zabbix-Monitoring-Lab-Deployment-Configuration
📌 Project Overview
This project demonstrates the successful deployment of a Zabbix 7.0 monitoring solution on an Ubuntu 24.04 server. The goal was to build a functional NOC (Network Operations Center) monitoring core to track system health and performance.

🛠️ Tech Stack
Operating System: Ubuntu 24.04 LTS

Database: MariaDB (MySQL-compatible)

Web Server: Apache2

Monitoring Software: Zabbix 7.0

🚀 Installation & Configuration Highlights
1. Database Backend
Initialized a MariaDB database and user with appropriate permissions.

Imported the Zabbix server schema using zcat to create the required table structures.

2. Troubleshooting (Critical Skill)
Problem: Encountered ERROR 1050 (42S01): Table 'role' already exists during schema import.

Solution: Performed a "Clean Slate" reset by dropping the database and recreating it to ensure no corrupted or duplicate tables existed.

3. Frontend Setup
Configured PHP settings including memory_limit, max_execution_time, and timezone synchronization (Asia/Kolkata).

Completed the web-based handshake to connect the Apache frontend to the MariaDB backend.

📈 Monitoring Capabilities
System Status: Monitoring the Zabbix server's internal health (CPU, RAM, and Disk usage).

Database Health: Real-time tracking of SQL performance and table status.
