# CLOUD STORAGE SETUP

**COMPANY**:  CODTECH IT SOLUTIONS

**NAME**:     GAYATHRI.N

**INTERN ID**: CT08NPC

**DOMAIN**: CLOUD COMPUTING

**DURATION**: 4 WEEKS

**MENTOR**: NEELA SANTHOSH KUMAR

**DESCRIPTION**:CODTECH IT SOLUTIONS
CLOUD COMPUTING INTERNSHIP
TASK-1: Cloud Storage Setup on AWS S3

1. Introduction
Amazon Simple Storage Service (AWS S3) is a highly scalable cloud storage solution that enables users to store and retrieve data efficiently. This report outlines the process of setting up an AWS S3 bucket, uploading files, and configuring the necessary access permissions to manage the storage securely.

2. Implementation Steps

Step 1: Create an S3 Bucket
The first step in the process is creating a new S3 bucket for storing files. The steps involved are:

Log in to the AWS Management Console.
Navigate to S3 and select the service.
Click the "Create Bucket" button.
Enter a unique bucket name, for example, my-cloud-storage-project.
Choose an appropriate AWS region where the bucket will be hosted.
Configure the Block Public Access Settings based on the requirements.
Click "Create Bucket" to finalize the creation.

Step 2: Upload Example Files
Once the bucket is created, the next step is to upload example files for testing purposes:

Open the newly created S3 bucket.
Click on the "Upload" button.
Select "Add Files" and choose files such as example.txt or image.jpg.
Click "Upload" to transfer the files into the S3 bucket.

Step 3: Configure Access Permissions
Configuring permissions ensures the appropriate access control for the files. In this case, public read access is configured:

Go to the Permissions tab of the bucket.
Under "Bucket Policy", click "Edit".
Add the following JSON policy to allow public read access:
json
Copy
Edit
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::my-cloud-storage-project/*"
    }
  ]
}
Click "Save Changes" to apply the policy.
3. Verification and Testing
To ensure everything was set up correctly, the following verifications were performed:

The S3 bucket was created successfully.
Example files were uploaded without any issues.
The access permissions were correctly configured.
The bucket policy for public read access was successfully applied (if required).
4. Conclusion
This report describes the steps taken to set up and configure an AWS S3 bucket, upload files, and configure access permissions. The process ensures secure file storage with the necessary controls for public or private access as required. This setup can be further optimized with additional features like lifecycle policies or encryption for enhanced security.
