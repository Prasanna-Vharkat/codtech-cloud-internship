
---

## 📁 Task-2-CloudWatch/README.md

```markdown
# 📊 Task 2 – Cloud Monitoring and Alerts (AWS CloudWatch)

## ✅ Objective:
Set up monitoring and alerting for a cloud-based application using **AWS CloudWatch**, with a custom dashboard and email-based alerts.

---

## 🛠️ Tools Used:
- AWS EC2 (monitored instance)
- AWS CloudWatch (metrics, dashboards, alarms)
- Amazon SNS (for email notifications)

---

## 📊 Monitored Resource:
- **EC2 Instance**
  - Metric: `CPUUtilization`

---

## 🧪 Alarm Configuration:
- Alarm Name: `EC2-CPU-Alert`
- Condition: `CPUUtilization > 50%` for 1 datapoint in 5 minutes
- Action: Sends email via SNS topic when triggered
- Additional Alarm: Billing alert for charges > $1

---

## 📸 Screenshots:
- CloudWatch dashboard
- Alarm creation
- SNS email confirmation
- Billing alarm view

📂 Stored in: `screenshots/`

---

## 📨 Email Alert Confirmation:
An email alert was successfully set up and verified using SNS subscription.

---

## 📝 Outcome:
- Gained experience in AWS CloudWatch dashboards and alarms
- Learned how to use SNS for cost-free alerting
- Demonstrated billing awareness via cost alarm

