# CloudSploit For Microsoft Azure

## Cloud Provider Configuration
1. Log into your Azure Portal and navigate to the Azure Active Directory service.
1. Select App registrations and then click on New registration.
1. Enter "CloudSploit" and/or a descriptive name in the Name field, take note of it, it will be used again in step 3.
1. Leave the "Supported account types" default: "Accounts in this organizational directory only (YOURDIRECTORYNAME)".
1. Click on Register.
1. Copy the Application ID and Paste it below.
1. Copy the Directory ID and Paste it below.
1. Click on Certificates & secrets.
1. Under Client secrets, click on New client secret.
1. Enter a Description (i.e. CloudSploit) and select Expires "In 1 year".
1. Click on Add.
1. The Client secret value appears only once, make sure you store it safely.
1. Navigate to Subscriptions.
1. Click on the relevant Subscription ID, copy and paste the ID below.
1. Click on "Access Control (IAM)".
1. Go to the Role assignments tab.
1. Click on "Add", then "Add role assignment".
1. In the "Role" drop-down, select "Security Reader".
1. Leave the "Assign access to" default value.
1. In the "Select" drop-down, type the name of the app registration (e.g. "CloudSploit") you created and select it.
1. Click "Save".
1. Repeat steps 13 to 21 for the roles "Log Analytics Reader", "Storage Account Key Operator Service Role" and "Key Vault Contributor"
1. Navigate to the "Key Vault" service
1. For each vault, select the vault name
1. Under "Settings" select the "Access Policies" blade
1. Select "Add an Access Policy"
1. Under "Key Permissions," "Secret Permissions," and "Certificate Permissions," select "List"
1. Under "Select service principal" select the name of the application (e.g. "CloudSploit")
1. Select "Add"
