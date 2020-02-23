# AlwaysOn-Performance-Dashboard

Data Collection
1. Setup.sql
This T-SQL script creates the schema (rpt), objects and SQL Agent Jobs required for performance data collection. This script need to be ran on all the sql instance which needs to be monitored. You also can use this dashboard to monitor CPU, DISK and RAM even with no AG configured, but on this I recommend to take a look on https://docs.microsoft.com/en-us/archive/blogs/sql_server_team/sql-server-performance-baselining-reports-unleashed-for-enterprise-monitoring

2. Data Collection Steps for each SQL Instance to Monitor
Connect to SQL PRIMARY instance to monitor
Run setup.sql
Check SQL Agent JOBs History to see if it runs successfully
Repeat for each SECONDARY Instance you want to monitor 
Deploying the reports to a file share or to the local disk of one of the SQL instances
On SSMS, register the dashboard report "AlwaysOn Performance Dashboard" as an Custom reports...


DISCLAIMER: The sample scripts and dashboard are provided AS IS without warranty or support of any kind. The entire risk arising out of the use or performance of the sample scripts and documentation remains with you.

Change Notes;

