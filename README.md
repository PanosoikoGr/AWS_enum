# 🔐 AWS IAM & S3 Auditor

A Python-based AWS auditing tool that uses **Boto3** to provide comprehensive visibility into IAM identities, their permissions, and potential role assumptions. It also allows optional **S3 file downloads** and **Secrets Manager inspection**, making it a lightweight but powerful cloud security reconnaissance utility.

---

## 🛠 Features

- 🔍 **Identity Inspection**  
  Retrieves and prints details about the current IAM identity using STS.

- 📜 **IAM Policy Enumeration**  
  - Lists attached and inline policies for IAM users.  
  - Extracts group memberships and attached/inlined group policies.

- 🔐 **Secrets Discovery**  
  - Lists all secrets in AWS Secrets Manager.  
  - Retrieves and prints contents of each secret securely.

- 📦 **S3 Bucket Support**  
  - Downloads all objects from a specified bucket into a local directory.

- 🧪 **Assumable Role Detection**  
  - Analyzes trust policies of IAM roles to identify assumable roles based on your current identity.  
  - Attempts to assume those roles and logs results.

- 🧾 **Formatted JSON Output**  
  - Policies and secrets are printed with clear formatting for easy review and logging.

---

## 🧰 Requirements

- Python 3.x  
- `boto3`  
- AWS Access Key ID and Secret Access Key with appropriate IAM permissions

---

## 🚀 Usage

```bash
python aws_auditor.py
