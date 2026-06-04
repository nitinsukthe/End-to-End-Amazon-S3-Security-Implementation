# S3 Bucket Policy Analysis

## 1. Purpose
Bucket policies define access control rules for Amazon S3 resources. This project uses a least-privilege policy to restrict access to a specific IAM user.

---

## 2. Policy Used

```json
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "DenyInsecureTransport",
            "Effect": "Deny",
            "Principal": "*",
            "Action": "s3:*",
            "Resource": [
                "arn:aws:s3:::nitin-cloud-security-s3-lab",
                "arn:aws:s3:::nitin-cloud-security-s3-lab/*"
            ],
            "Condition": {
                "Bool": {
                    "aws:SecureTransport": "false"
                }
            }
        }
    ]
}
