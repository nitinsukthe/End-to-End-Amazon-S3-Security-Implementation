# Versioning & Data Recovery Test

## 1. Overview
S3 Versioning is used to protect against accidental deletion or overwriting of objects by maintaining historical versions.

---

## 2. Configuration Steps
- Navigate to S3 bucket properties
- Enable "Bucket Versioning"
- Confirm activation

---

## 3. Test Scenario

### Step 1: Upload File
- Upload test file to bucket

### Step 2: Modify File
- Upload modified version with same filename

### Step 3: Delete File
- Delete object from bucket

---

## 4. Recovery Process
- Enable "Show Versions"
- Identify previous object versions
- Restore required version

---

## 5. Security Impact
- Prevents permanent data loss
- Supports ransomware recovery scenarios
- Maintains data integrity
