# AWS Resource Tracker

A Python boto3 tool that scans your entire AWS account,
lists all running resources, and generates a cost
report exported to CSV.

---

## What It Does

- Scans EC2, S3, RDS, Lambda across all regions
- Shows running vs stopped resources
- Calculates cost per resource via Cost Explorer API
- Exports full report to CSV
- Sends summary email via SNS

---

## Tech Stack

- Python 3
- boto3 (AWS SDK)
- AWS Cost Explorer API
- AWS SNS
- AWS Lambda + EventBridge (scheduled)

---

## How to Run

```bash
git clone https://github.com/nithishkt2608/aws-resource-tracker
cd aws-resource-tracker
pip install boto3
python tracker.py
```

---

## Sample Output
ServiceResource IDStatusMonthly CostEC2i-0abc123Running$8.50RDSdb-prodRunning$15.20S3my-bucketActive$0.45Lambdacost-funcActive$0.00

---
Built by Nithishkannan | MCS @ Illinois Tech
