# 📦 Task 1 – Cloud Storage Setup (AWS S3)

## ✅ Objective:
Create and configure cloud storage using **AWS S3**, upload example files, and apply correct access permissions, including one **public** and one **private** object.

---

## 🛠️ Tools Used:
- AWS Management Console (S3)
- JSON Bucket Policy Editor
- GitHub for documentation

---

## 📁 Bucket Details:
- **Bucket Name**: `codtech-task1-prasanna`
- **Region**: us-east-1 (N. Virginia)
- **Access**:
  - Entire bucket: Public
  - One file (`AWS_S3.txt`): Explicitly **denied** public access using bucket policy

---

## 🔐 Bucket Policy Summary:
```json
{
  "Sid": "DenyPublicAccessToSpecificFile",
  "Effect": "Deny",
  "Principal": "*",
  "Action": "s3:GetObject",
  "Resource": "arn:aws:s3:::codtech-task1-prasanna/AWS_S3.txt"
}
