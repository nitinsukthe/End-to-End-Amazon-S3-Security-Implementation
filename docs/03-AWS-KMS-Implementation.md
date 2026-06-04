# AWS KMS Implementation

## Objective

Protect sensitive data stored in Amazon S3 using server-side encryption with AWS Key Management Service (KMS).

---

## Implementation Steps

1. Created a customer-managed KMS key
2. Assigned alias:
   s3-security-key
3. Enabled Default Encryption on the S3 bucket
4. Selected AWS KMS (SSE-KMS)
5. Applied encryption configuration

---

## Encryption Model

S3 Object
    ↓
AWS KMS Key
    ↓
Encrypted Storage

---

## Security Benefits

### Data Confidentiality

Protects stored data from unauthorized access.

### Centralized Key Management

Allows encryption key monitoring and management.

### Compliance Support

Supports common cloud security and compliance requirements.

### Auditability

KMS usage can be monitored through AWS logging services.

---

## Result

All newly uploaded objects are encrypted automatically using AWS KMS.
