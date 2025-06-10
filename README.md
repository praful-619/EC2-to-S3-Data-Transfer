# Seamless EC2 to S3 Data Transfer with Real-Time Alerts Using Amazon SNS

Discription 
In this project, we automate the process of transferring files from an Amazon EC2 instance to an S3 bucket and integrate Amazon SNS (Simple Notification Service) for real-time alerts. The goal is to ensure that any data generated or collected on EC2—such as logs, backups, reports, or media—is reliably pushed to Amazon S3 for secure, durable storage.
To monitor and ensure visibility into the data transfer process, an SNS topic is configured to send real-time email or SMS notifications when:
A file is successfully uploaded to S3
A transfer fails or encounters an error
This setup supports production-ready use cases like:
Backup automation
Log aggregation
Application data archival
All components are configured using AWS CLI, IAM roles for secure access, and cron jobs (or scripts) on EC2 for automation.

Technologies
EC2 Instance: Source of data (files/logs/etc.)
Amazon S3: Destination storage
Amazon SNS: Alerting mechanism (email/SMS)
IAM Roles/Policies: Secure and scoped access control
Shell Scripts/Cron Jobs: Automate file upload and notification trigger

Results
✅ Files from EC2 are automatically uploaded to the designated S3 bucket.
✅ An SNS notification (email/SMS) is sent instantly upon success or failure.
✅ The entire process is fully automated and secure via IAM.
✅ Real-time visibility into data movement ensures operational transparency.
✅ Scalable solution for future workloads without manual intervention.



