# Welcome to Veeam Solution for OMS

This free Intelligent Pack for Operations Management Suite allows you to monitor:

- Veeam Backup & Replication Server
- Veeam Agent for Windows
- Veeam Agent for Linux

For Veeam B&R, you can view performance monitor about CPU, Memory and Disk; for Veeam Agent you can view service status of main service.

Get Started

Before import the solution, you must create a group called GroupComputerVeeamBackup, with this query:

Event
| where EventLog == "Veeam Backup"
| distinct Computer

The project is open and everyone can improve the IP. For more information you send a feedback from our web page: www.insidetechnologies.eu.
