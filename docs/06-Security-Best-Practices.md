# AWS S3 Security Best Practices

## 1. Access Control
- Enable "Block Public Access" at bucket level
- Use IAM roles instead of root access
- Apply least privilege policies

---

## 2. Encryption
- Enable SSE-KMS for all buckets
- Rotate KMS keys regularly
- Enforce encryption via bucket policy

---

## 3. Monitoring & Logging
- Enable S3 access logs
- Enable AWS CloudTrail
- Monitor unauthorized access attempts

---

## 4. Data Protection
- Enable versioning
- Enable MFA delete (if required)
- Use lifecycle policies for backups

---

## 5. Operational Security
- Avoid hardcoded credentials
- Use IAM roles for automation
- Regularly audit permissions
