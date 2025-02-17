# AWS Resource Listing Automation (Shell Script)

## Overview  
This project provides a **Bash script** to automate the process of listing various **AWS resources** in a given AWS region. Instead of manually running AWS CLI commands, this script streamlines the process and ensures efficiency.  

It supports multiple AWS services, including **EC2, S3, RDS, IAM, Lambda, Route53, CloudFront, DynamoDB, and more.**  

---

## Features  
✅ Lists AWS resources dynamically based on user input  
✅ Supports multiple AWS services (EC2, S3, RDS, Lambda, etc.)  
✅ Validates AWS CLI installation and configuration before execution  
✅ Provides **clear and structured output** for each AWS service  
✅ Includes error handling for **invalid services or misconfigurations**  

---

## 🔧 Prerequisites  
Before running the script, ensure you have the following:  

1️⃣ **AWS CLI Installed**:  
   - Check if AWS CLI is installed:  
     ```bash
     aws --version
     ```
   - If not installed, follow [AWS CLI Installation Guide](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html).  

2️⃣ **AWS CLI Configured**:  
   - Run the following command to configure credentials:  
     ```bash
     aws configure
     ```
   - Enter:  
     - AWS Access Key  
     - AWS Secret Key  
     - Default AWS region  
     - Output format (json, table, text)  

3️⃣ **Bash Shell**:  
   - The script is designed to run in **Linux/macOS/WSL (Windows Subsystem for Linux).**  
   - If using Windows, install Git Bash or WSL.  

---

## Installation  

Clone this repository to your local system:  

```bash
git clone https://github.com/GUPTHA-MADDULA/Shell_Scripting.git
cd Shell_Scripting

# Ensure your script has execution permissions
chmod +x aws_resource_list.sh

#Usage:
#Basic Usage
Run the script by specifying the AWS region and service name:

./aws_resource_list.sh <aws_region> <aws_service>

#Example Commands:

1. List EC2 Instances in us-east-1:
./aws_resource_list.sh us-east-1 ec2



