# AWS VPC and S3 Integration Project  

## Project Overview  
This project demonstrates the integration of Amazon VPC and S3 using an EC2 instance. The objective was to create a secure, isolated environment to run an application, connect to an EC2 instance, and access an S3 bucket using a VPC endpoint.  

## Key Features  
- **Amazon VPC Setup**: Created a Virtual Private Cloud (VPC) to ensure a secure and isolated network.  
- **EC2 Instance Launch**: Deployed an EC2 instance into the VPC to serve as the compute resource.  
- **S3 Bucket Configuration**: Created and configured an S3 bucket named `nextwork-vpc-project-arjun` for file storage and data transfer.  
- **VPC Endpoint**: Established a VPC endpoint for secure, private access to S3, eliminating the need for public exposure.  
- **AWS CLI Commands**: Used AWS CLI to interact with S3, including uploading and listing files.  

## Project Workflow  
1. **Architecture Setup**  
   - Launched a VPC and deployed an EC2 instance.  
   - Configured networking, subnets, and security groups.  
2. **EC2 Instance Access**  
   - Connected to the EC2 instance directly using SSH.  
   - Installed AWS CLI for seamless interaction with AWS services.  
3. **S3 Bucket Setup**  
   - Created an S3 bucket and uploaded files such as:  
     - `NextWork - Denzel is awesome.png`  
     - `NextWork - Lelo is awesome.png`  
   - Verified the uploaded files using AWS CLI.  
4. **File Uploads via CLI**  
   - Created a new file (`nextwork.txt`) on the EC2 instance.  
   - Uploaded the file to the S3 bucket using:  
     ```bash
     aws s3 cp /tmp/nextwork.txt s3://nextwork-vpc-endpoints-arjun
     ```  
   - Verified successful upload using:  
     ```bash
     aws s3 ls s3://nextwork-vpc-endpoints-arjun
     ```  

## Tools and Technologies  
- **Amazon Web Services (AWS)**  
  - Amazon VPC  
  - Amazon EC2  
  - Amazon S3  
  - VPC Endpoint  
- **AWS CLI**: Used for managing AWS resources.  

## Challenges and Learnings  
- **Challenge**: Configuring the security settings for the VPC endpoint was more complex than expected.  
- **Learning**: Gained deeper insights into VPC endpoint configurations and enhanced project security.  

## Time Taken  
The project was completed in approximately **1.5 hours**, including configuration and troubleshooting.  
