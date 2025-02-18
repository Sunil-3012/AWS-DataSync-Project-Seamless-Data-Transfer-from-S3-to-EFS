# AWS DataSync Project: Seamless Data Transfer from S3 to EFS  

## Overview  
Designed and implemented a **secure and automated data transfer solution** using **AWS DataSync**, enabling seamless **migration of data from Amazon S3 to Amazon Elastic File System (EFS)**. This setup ensures **scalability, high availability, and efficient data synchronization** while reducing operational overhead.  


## Technologies Used  
- **AWS DataSync** – Automates data movement from S3 to EFS.  
- **Amazon EC2** – Hosts the DataSync agent for data transfer.  
- **Amazon S3** – Source storage for data objects.  
- **Amazon EFS** – Destination for scalable file storage.  
- **AWS IAM** – Manages secure access control.  
- **AWS CloudWatch** – Monitors data transfer performance.  

## Features  
✔ **Automated, high-speed data transfer from S3 to EFS.**  
✔ **Scalable and highly available storage solution.**  
✔ **Secure IAM access control for data integrity.**  
✔ **CloudWatch monitoring for real-time tracking.**  

---

## Implementation  

### **1. Source and Destination Setup**  
- Created a **secure S3 bucket** with **private access** for storing sample data.  
- Provisioned an **Amazon EFS file system** as the **destination storage**, ensuring **scalability and high availability**.  

### **2. DataSync Agent Deployment**  
- Launched an **EC2 instance** using the **AWS DataSync Agent AMI** to act as an intermediary.  
- Configured **security groups** to allow necessary protocols (**NFS, SSH, HTTP**) for secure communication between **S3 and EFS**.  

### **3. Task Configuration in AWS DataSync Console**  
- Created and registered the **DataSync Agent** in the **AWS Management Console**.  
- Defined **Source Location** as **S3 bucket** and **Destination Location** as **EFS file system**.  
- Configured and ran the **DataSync task**, leveraging **AWS DataSync's optimized performance**, which enables transfers **up to 10x faster than traditional methods**.  

### **4. Data Validation**  
- Deployed another **EC2 instance** and mounted the **EFS file system** using the `nfs-utils` package.  
- Validated **successful data transfer** by listing and verifying files within the mounted **EFS directory**.  

### **5. Benefits Delivered**  
- Eliminated **manual data transfer processes**, reducing **operational overhead** and improving efficiency.  
- Leveraged **AWS DataSync’s automation** for **scripting, scheduling, and monitoring**, ensuring **reliable and consistent data migration**.  
- Achieved a **cost-effective, scalable, and fully managed solution** for **seamless cloud-based file synchronization**.  

---

## Outcome  
- Successfully implemented **secure, automated, and high-speed data transfer** from **S3 to EFS**.  
- Ensured **data integrity and high availability** with **AWS IAM access control**.  
- Optimized transfer efficiency using **AWS DataSync automation**.  

### **Screenshots**  

#### **1. AWS DataSync Task Excution on CLI**  
![DataSync Task CLI](/Users/gangupamusaisunil/AWS/projects/dataSync/DataSync-cli.jpeg)  

#### **2. Data Transfer Progress in AWS Console**  
![Data Transfer Progress](path/to/data-transfer-progress.png)  

#### **3. Validated Data in Mounted EFS Directory**  
![EFS Data Validation](path/to/efs-data-validation.png)  

## Repository Structure  
  


## Future Enhancements  
- Implement **CloudWatch Alarms** for **real-time failure detection**.  
- Enable **AWS Lambda triggers** to automate post-transfer actions.  
- Integrate **SNS notifications** for event-based updates.  

This project showcases expertise in **AWS DataSync, automated cloud data migration, IAM security, and scalable storage solutions**. 🚀  
 
 
