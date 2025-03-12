# wordpress-website
# AWS WordPress Deployment

## Description
This project documents the deployment of a WordPress website on AWS using EC2, VPC, and RDS.

## AWS Services Used
- **EC2**: Hosts the WordPress application  
- **RDS (MySQL)**: Manages the database  
- **VPC**: Configures networking for security  
- **S3 (Optional)**: Stores media files  
- **Route 53 (Optional)**: Manages custom domain  

## Deployment Steps

### Step 1: Launch EC2 Instance
1. Created an EC2 instance with Amazon Linux 2.  
2. Installed Apache, PHP, and MySQL client.  
3. Configured security groups for HTTP (80) and SSH (22).  

### Step 2: Set Up RDS (MySQL)
1. Created an RDS instance with MySQL.  
2. Enabled public accessibility.  
3. Connected EC2 to RDS using MySQL credentials.  

### Step 3: Configure VPC
1. Created a custom VPC with subnets.  
2. Configured Internet Gateway and Route Table.  
3. Associated EC2 and RDS with the VPC.  

### Step 4: Install WordPress
1. Downloaded WordPress and extracted it in `/var/www/html/`.  
2. Configured `wp-config.php` to connect to RDS.  
3. Set file permissions and restarted Apache.  

### Live Website  
[Visit Website](http://your-public-ip-or-domain)

## Screenshots
![EC2 Instance](screenshots/ec2-instance.png)  
![RDS Setup](screenshots/rds-setup.png)  

## Author  
Your Name  
