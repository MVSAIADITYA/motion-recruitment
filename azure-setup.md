1. Create an Azure Account
Visit Azure Website: Go to the Azure website.
Initiate Sign Up: Click on “Start free” or “Create an Azure free account”.
Provide Personal Information: Enter your personal details, including name, email, and phone number.
Identity Verification: Verify your identity via SMS or phone call with a verification code.
Payment Information: Enter your credit/debit card details. (Note: You won't be charged for the free tier, but card information is required.)
Complete Registration: Finish the setup and log in to the Azure portal.
2. Log In to Azure Portal
Access the Portal: Navigate to the Azure Portal.
Sign In: Log in using your new Azure account credentials.
3. Set Up a Basic Azure Virtual Machine (VM)
Navigate to Virtual Machines: In the Azure Portal, use the search bar to find and select "Virtual Machines".
Create VM:
Click on “+ Add” and then “+ Virtual machine”.
Basic Configuration:
Subscription: Select your subscription plan.
Resource Group: Create a new resource group or use an existing one.
Virtual machine name: Enter a name for your VM.
Region: Choose a region close to your location.
Image: Select an image, such as Ubuntu Server.
Size: Choose an appropriate size (e.g., B1s for a low-cost VM).
Administrator Account:
Authentication Type: Choose SSH public key.
Username: Enter a username.
SSH Public Key: Paste your public SSH key or generate a new one using SSH-keygen.
Disks Configuration: Configure disk options, generally, the default settings are sufficient.
Networking: Ensure the network settings allow SSH (port 22).
Management, Advanced, and Tags Sections: Configure additional settings if needed, otherwise, leave default.
Review and Create:
Review all configurations.
Click “Create” to deploy the VM.
4. Connect to Your Azure VM
Access the VM: Go to the "Virtual Machines" section in the Azure Portal and select your VM.
Get Public IP Address: Note the public IP address of your VM.
SSH Access:
Open a terminal (or use PuTTY on Windows if needed).
Use SSH to connect: ssh username@public-ip-address (replace with your VM username and IP).
5. Deploy a Sample Python Script
Update VM & Install Python:
Update the VM's package lists: sudo apt update.
Install Python 3: sudo apt install python3.
Upload or Create Python Script:
Create a new Python script using a text editor (e.g., nano or vim): nano add_numbers.py.
Write a simple script to add two numbers (e.g., print(1 + 2)).
Save and close the editor.
Run the Script:
Execute the script: python3 add_numbers.py.
6. Verify Output
Check Script Execution: Confirm the script output to ensure it runs correctly.
Troubleshoot if Necessary: Resolve any issues if the script does not run as expected.
