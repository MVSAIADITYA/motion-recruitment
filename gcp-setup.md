1. Create a GCP Account
Visit GCP Website: Go to the Google Cloud Platform website.
Initiate Sign Up: Click on “Get started for free”.
Provide Google Account: Sign in with your existing Google account or create a new one.
Accept Terms: Read and accept the terms of service.
Fill in Account Information: Provide your personal details such as name and address.
Payment Information: Enter your credit/debit card details. (Note: GCP provides a free trial with credits, but card information is required.)
Identity Verification: Complete any required identity verification processes.
Complete Registration: Finish the setup and wait for account activation.
2. Log In to Google Cloud Console
Access Google Cloud Console: Navigate to the Google Cloud Console.
Sign In: Use your Google account credentials to log in.
3. Set Up a Google Compute Engine Instance
Navigate to Compute Engine: In the Google Cloud Console, use the navigation menu to find and select "Compute Engine".
Enable Compute Engine API: If prompted, enable the Compute Engine API.
Create an Instance:
Click on “Create Instance”.
Configure Instance:
Name: Enter a name for your instance.
Region and Zone: Select a suitable region and zone.
Machine Type: Choose an appropriate machine type (e.g., e2-micro for the free tier).
Boot Disk: Select an operating system, such as Debian or Ubuntu.
Firewall:
Allow HTTP and HTTPS traffic if needed.
Identity and API Access: Configure instance permissions if necessary.
Management, Security, Disks, Networking, Sole Tenancy: Configure additional settings as required or leave default settings.
Review and Create:
Review all configurations.
Click “Create” to deploy the instance.
4. Connect to Your Compute Engine Instance
Access the Instance: Go to the "VM instances" section in the Compute Engine dashboard.
Connect via SSH:
Click on the SSH button next to your instance to open an SSH terminal directly in the browser.
Alternatively, use the provided SSH command to connect from a local terminal if SSH keys are configured.
5. Deploy a Sample Python Script
Update Instance & Install Python:
Update the instance’s package lists using the package manager (e.g., apt for Debian/Ubuntu).
Install Python 3 using the package manager.
Upload or Create Python Script:
Use a text editor (e.g., nano or vim) to create a new Python script file (e.g., add_numbers.py).
Write a simple Python script to add two numbers (e.g., print(1 + 2)).
Save and exit the editor.
Run the Script:
Execute the script using Python 3.
6. Verify Output
Check Script Execution: Confirm the script output to ensure it runs correctly.
Troubleshoot if Necessary: Resolve any issues if the script does not run as expected.
