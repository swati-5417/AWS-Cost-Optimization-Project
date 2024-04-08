# Cost-Optimization-Project
EBS Snapshot Cleanup using Lambda Function

This project involves creating a Lambda function to help manage storage costs on AWS. The function automatically identifies and deletes unused EBS snapshots, which are essentially backups of data stored on Amazon's Elastic Block Store (EBS).

How It Works:

The Lambda function first gathers all EBS snapshots owned by the AWS account.
It then checks if the associated EBS volumes are not connected to any active EC2 instances (servers).
If a snapshot is found to be unused, the function deletes it, thereby saving on storage costs.
Why It's Useful:

By removing unnecessary snapshots, this function helps optimize storage resources, reducing AWS billing costs.
It automates the cleanup process, saving time and effort for AWS users.
Key Technologies Used:

AWS Lambda: Serverless computing service used to execute the cleanup function.
AWS EC2: Service providing resizable compute capacity in the cloud, where instances may use EBS volumes.
AWS EBS: Block-level storage volumes used with EC2 instances.
How to Use:

Simply deploy the Lambda function in your AWS environment and configure it to run on a schedule or trigger event.
