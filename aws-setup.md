Step 1: Create an AWS Account
Navigate to the AWS Website: Go to AWS website.
Click on "Create an AWS Account": This will redirect you to the sign-up page.
Fill in Account Information: Enter your email address, password, and AWS account name.
Provide Contact Information: Submit your personal details such as name, phone number, and address.
Payment Information: Enter your credit/debit card details. AWS has a free tier, but card information is required for account creation.
Identity Verification: Complete the identity verification process through a phone call or SMS.
Select Support Plan: Choose a support plan. You can select the free Basic plan if you're just getting started.
Complete Setup: Click "Complete Sign Up". You might need to wait for a few minutes to receive a confirmation email.
Step 2: Log In to AWS Management Console
Login: Visit the AWS Management Console and log in using the account you just created.
Dashboard: You’ll be taken to the AWS Management Console Dashboard.
Step 3: Set Up a Basic EC2 Instance
Launch EC2 Dashboard: In the AWS Management Console, search for and select "EC2" to open the EC2 Dashboard.
Launch Instance: Click on "Launch Instance".
Choose an Amazon Machine Image (AMI): Select an AMI (e.g., Amazon Linux 2 AMI).
Choose Instance Type: Select an instance type (e.g., t2.micro, which is free-tier eligible).
Configure Instance Details: Set the number of instances and other configurations. Usually, the default settings are sufficient for basic setup.
Add Storage: Configure storage options if necessary, otherwise leave the default settings.
Add Tags: Add tags for organization if needed.
Configure Security Group:
Create a new security group.
Add rules to allow SSH (port 22) and HTTP (port 80) access.
Review and Launch: Review all configurations, then click "Launch".
Select Key Pair: Choose to create a new key pair or use an existing one. Download the key pair .pem file.
Launch: Click "Launch Instances".
Step 4: Connect to Your EC2 Instance
Access Instance Details: Navigate back to the EC2 Dashboard and find your running instance.
Get Public IP: Note the public IP address or public DNS of the instance.
SSH Connection:
Open a terminal (or use PuTTY on Windows).
Navigate to the directory where your key pair .pem file is stored.
Use SSH to connect: ssh -i "your-key-pair.pem" ec2-user@your-instance-public-ip.
Step 5: Deploy a Sample Python Script
Install Python (if not pre-installed):
Update the package lists: sudo yum update -y.
Install Python 3: sudo yum install python3 -y.
Upload Your Script:
Create a new Python file: nano add_numbers.py.
Write a script to add two numbers. (E.g., print(1 + 2)).
Save and exit the editor.
Run Your Script:
Execute the script: python3 add_numbers.py.
Step 6: Confirm Execution
Verify Output: Check the console for the expected output from your Python script 