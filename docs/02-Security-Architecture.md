# Security Architecture: Amazon S3 Secure Storage Design

## 1. Architecture Overview
This architecture ensures secure storage of objects in Amazon S3 using layered security controls.

---

## 2. Components

### Amazon S3 Bucket
Primary storage layer for objects with restricted access.

### IAM (Identity and Access Management)
Controls who can access the bucket and what actions they can perform.

### AWS KMS (Key Management Service)
Provides encryption keys for server-side encryption of objects.

### S3 Versioning
Maintains object history for recovery and rollback.

### Access Logging
Captures request-level logs for auditing and monitoring.

---

## 3. Security Layers

### Layer 1: Network & Access Control
- Public access blocked
- IAM-based authentication enforced

### Layer 2: Data Protection
- Server-side encryption using AWS KMS (SSE-KMS)

### Layer 3: Data Integrity
- Versioning enabled to prevent accidental deletion or overwrite loss

### Layer 4: Monitoring
- S3 access logs enabled for forensic analysis

---

## 4. Security Flow
1. User authenticates via IAM
2. Requests are validated against bucket policy
3. Data is encrypted using KMS before storage
4. All actions are logged for auditing
