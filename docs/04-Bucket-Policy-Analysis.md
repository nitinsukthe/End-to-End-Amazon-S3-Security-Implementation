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
      "Effect": "Allow",
      "Principal": {
        "AWS": "arn:aws:iam::123456789012:user/username"
      },
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::my-secure-bucket/*"
    }
  ]
}
