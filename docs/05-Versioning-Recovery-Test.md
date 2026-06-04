# Versioning Recovery Test

## Objective

Validate Amazon S3 Versioning functionality and demonstrate data recovery capabilities.

---

## Test Scenario

### Version 1

Uploaded:

confidential-data.txt

Version ID generated automatically by Amazon S3.

---

### Version 2

Modified file contents.

Re-uploaded file to the bucket.

Amazon S3 generated a second Version ID.

---

## Verification

Enabled:

Show Versions

Observed:

- Original object version
- Updated object version

Both versions remained available.

---

## Security Benefits

### Accidental Deletion Recovery

Previous versions remain accessible.

### Ransomware Protection

Encrypted or modified files can be restored.

### Change Tracking

Provides object history.

### Data Integrity

Protects against unintended modifications.

---

## Test Result

Versioning successfully preserved multiple object versions and validated recovery functionality.
