# Welcome to Veeam Solution for OMS

This free Intelligent Pack for Operations Management Suite allows you to monitor Veeam Backup & Replication Server and Veeam Agent. The project is open and everyone can improve the IP. For more information you send a feedback from our web page: www.insidetechnologies.eu.

What’s New in build 1.0.0.0:

- Veeam Backup & Replication Server Job Status
- Veeam Backup & Replication Server Performance Monitor about CPU, Memory and Disk
- Veeam Agent for Windows Service Status
- Veeam Agent for Linux Service Status

# Get Started

Before import the solution, you must create a group called GroupComputerVeeamBackup, with this query:

Event
| where EventLog == "Veeam Backup"
| distinct Computer

The second step is enable the Windows Event logs (Settings area) for Veeam Agent and Veeam Backup (Error, Warning, Information).
