# 📊 Task 2 – Cloud Monitoring and Alerts (AWS CloudWatch)

## ✅ Objective:
Set up monitoring and alerting for a cloud-based application using **AWS CloudWatch**, with:
- A custom dashboard displaying EC2 instance metrics
- CloudWatch alarms configured to send email alerts
- A billing alarm for AWS usage tracking

---

## 🧰 Tools Used:
- **AWS CloudWatch** (for metrics and alarms)
- **Amazon EC2** (monitored instance)
- **Amazon SNS** (for email notifications)
- **AWS Free Tier**

---

## 🔍 Monitored Resource:
- **EC2 Instance ID**: *(Instance ID used for CPU monitoring)*
- **Monitored Metric**: `CPUUtilization`  
- **Dashboard**: Custom dashboard created with a line widget showing live CPU usage

---

## 🔔 Alarm Configuration:

### 📌 Alarm 1: EC2 CPU Alert
- **Name**: `EC2-CPU-Alert`
- **Metric**: CPUUtilization
- **Condition**: CPU > 50% for 1 datapoint within 5 minutes
- **State**: OK (EC2 was idle)
- **Notification**: Email alert using Amazon SNS

### 📌 Alarm 2: AWS Billing Alert
- **Name**: `AWS TOTAL BILLING`
- **Metric**: `EstimatedCharges`
- **Condition**: Charges >= $1
- **State**: OK (billing under limit)
- **Purpose**: Prevent unexpected AWS charges

---

## 📨 Email Notification Setup:
- Created an SNS topic: `codtech-task2-alerts`
- Subscribed with email ID
- Confirmed subscription via email
- Alerts are triggered to email when alarm conditions are met

---

## 🖼️ Screenshots (Located in `screenshots/` folder):

| Screenshot                | Description                             |
|---------------------------|-----------------------------------------|
| `dashboard.png`           | CloudWatch dashboard with EC2 metrics   |
| `alarm-config.png`        | EC2-CPU alarm configuration             |
| `email-confirmation.png`  | SNS email subscription confirmation     |
| `alert-email.png` (opt.)  | Email received on alarm trigger         |
| `billing-alarm.png`       | AWS billing alarm configuration         |

---

## 📝 Outcome:
- Successfully monitored EC2 instance performance using CloudWatch
- Created real-time dashboards for visibility
- Configured and tested alarms with SNS email alerts
- Set up AWS billing alarm as a precaution

---

## 🙋 Intern Info:
- 👨‍💻 Name: Prasanna Anil Vharakat  
- 🆔 Intern ID: CT08DM450  
- 🏢 Organization: CODTECH IT Solutions Pvt. Ltd.  
- 📅 Duration: May 8, 2025 – July 8, 2025

---

> _“Monitoring is the foundation of reliability in the cloud. If you can't see it, you can't fix it.”_
