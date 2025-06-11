# ☁️ Seamless EC2 to S3 Data Transfer with Real-Time Alerts Using Amazon SNS

> 🔄 Automate data transfers from EC2 to S3 and receive instant notifications using Amazon SNS.

---

## 📘 Description

In this project, we **automate the process of transferring files** from an **Amazon EC2 instance** to an **Amazon S3 bucket**, while integrating **Amazon SNS (Simple Notification Service)** for **real-time alerts**.

The goal is to ensure that any data generated or collected on EC2—such as logs, backups, reports, or media—is **reliably and securely pushed to Amazon S3** for **durable cloud storage**.

---

### 🔔 Real-Time Monitoring with SNS

An **SNS topic** is configured to send **real-time email or SMS notifications** when:

- ✅ A file is **successfully uploaded** to S3  
- ❌ A transfer **fails or encounters an error**

---

## 🧩 Supported Use Cases

- 🔄 Backup Automation  
- 📑 Log Aggregation  
- 📁 Application Data Archival  

---

## 🧰 Technologies Used

| Component              | Purpose                                      |
|------------------------|----------------------------------------------|
| 🖥️ **EC2 Instance**        | Source of data (files, logs, etc.)            |
| 📦 **Amazon S3**          | Destination cloud storage                    |
| 📣 **Amazon SNS**         | Notification service for success/failure     |
| 🔐 **IAM Roles/Policies** | Scoped access and security for EC2 → S3/SNS |
| 🛠️ **Shell Scripts**       | File transfer & notification logic           |
| ⏰ **Cron Jobs**           | Scheduling automated execution               |

---

## ⚙️ How It Works

```text
[EC2 Instance] -- (Shell Script/Cron Job) --> [Amazon S3 Bucket]
                               ↘
                            [SNS Alert]
