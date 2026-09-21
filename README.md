# AWS S3 & Local Infrastructure Automation using Terraform

This repository demonstrates end-to-end Infrastructure as Code (IaC) management using *HashiCorp Terraform* and *Amazon Web Services (AWS)*. It covers local resource state management, AWS IAM authentication via AWS CLI v2, automated cloud provisioning, and safe resource lifecycle teardowns.

---

## 📌 Project Overview

* *Local State & Resource Management:* Configured, updated, and safely destroyed local file resources using the hashicorp/local provider while tracking state changes in terraform.tfstate.
* *Security & Authentication:* Installed AWS CLI v2 on Ubuntu Linux and configured IAM credentials (AmazonS3FullAccess) following identity best practices.
* *Cloud Infrastructure Automation:* Initialized the hashicorp/aws provider, generated execution plans (terraform plan), and provisioned an Amazon S3 bucket (neha-nikams-bucket) in the us-west-2 region.
* *Lifecycle Cleanup:* Verified active deployments in the AWS S3 Console and executed terraform destroy for clean, automated teardowns.

---

## 🛠️ Architecture & Tools Used

* *Infrastructure as Code:* HashiCorp Terraform (Providers: aws, local)
* *Cloud Provider:* Amazon Web Services (AWS S3, IAM)
* *CLI & Environment:* AWS CLI v2, Ubuntu Linux, Bash
* *Version Control:* Git & GitHub

---

## 📁 Repository Structure

```text
.
├── main.tf           # Provider configurations & local resource definitions
├── s3.tf             # AWS S3 bucket resource declarations
├── .gitignore        # Excludes terraform state files & temporary artifacts
└── README.md         # Project documentation
