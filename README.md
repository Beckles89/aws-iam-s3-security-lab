# AWS IAM & S3 Security Lab

## 🔐 Overview
This project demonstrates implementation of AWS Identity and Access Management (IAM) and secure S3 bucket configuration following the Principle of Least Privilege.

## 🎯 Objectives
- Create secure IAM users and groups
- Enforce least privilege access control
- Secure S3 bucket from public access
- Test access permissions across different roles

---

## 🛠️ Environment
- AWS IAM
- Amazon S3
- AWS Management Console

---

## 🔧 Steps Performed

### 1. Secured Root Account
- Enabled MFA
- Avoided use of root for daily tasks

---

### 2. Created Admin IAM User
- Username: `matt-admin`
- Assigned to `Admins` group
- Attached policy: `AdministratorAccess`

---

### 3. Created Secure S3 Bucket
- Bucket name: `matt-secure-bucket-2026`
- Blocked all public access
- Enabled encryption (default)

---

### 4. Uploaded Test File
- Uploaded `.docx` file to S3
- Verified storage functionality

---

### 5. Created Limited IAM User
- Username: `bob-test`
- Assigned restricted permissions

---

### 6. Implemented Least Privilege Policy
- Allowed:
  - `s3:GetObject`
- Denied:
  - Upload
  - Delete
  - IAM access

---

### 7. Access Testing

#### Admin User
- Full access to IAM and S3 ✅

#### Non-Admin User (bob-test)
- Can download files ✅
- Cannot upload files ❌
- Cannot delete files ❌
- Cannot access IAM ❌

---

## 🔍 Key Security Concepts Demonstrated
- Principle of Least Privilege
- Identity-Based Policies
- Access Control Enforcement
- Secure Cloud Storage Configuration

---

## 📸 Screenshots
(Add your screenshots here)

---

## 📈 Skills Gained
- AWS IAM Configuration
- Access Control Design
- Cloud Security Fundamentals
- Security Testing & Validation
