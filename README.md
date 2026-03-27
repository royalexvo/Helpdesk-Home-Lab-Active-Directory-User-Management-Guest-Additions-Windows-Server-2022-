<h1>Helpdesk Home Lab – Active Directory User Management & Guest Additions (Windows Server 2022)</h1>

<h2>Description</h2>
This lab continues the HelpDesk Home Lab series by introducing basic Active Directory user management and improving virtual machine usability with Guest Additions.

<br />In this lab, the following tasks were completed:
- <b>Log into Windows Server 2022 as Administrator</b>
- <b>Install VirtualBox Guest Additions for file transfer capability</b>
- <b>Configure shared folders between host and VM</b>
- <b>Access and navigate Active Directory Users and Computers</b>
- <b>Create new user accounts in Active Directory</b>
- <b>Modify user account properties (address, department, etc.)</b>
- <b>Manage user account settings (reset password, disable/enable, unlock)</b>
- <b>Configure logon hours and user restrictions</b>
- <b>Verify user accounts using command line tools</b>

This builds on the previous lab where Active Directory Domain Services (AD DS) was installed.
<br />

<h2>Languages and Utilities Used</h2>

- <b>Windows Server 2022</b>
- <b>Active Directory Users and Computers (ADUC)</b>
- <b>Oracle VirtualBox (Guest Additions)</b>
- <b>Command Prompt (CMD)</b>
- <b>net user command</b>

<h2>Environments Used </h2>

- <b>Host Operating System: Windows 10 / Windows 11</b>
- <b>Virtualization Platform: Oracle VirtualBox</b>
- <b>Guest Operating System: Windows Server 2022</b>

<h2>Program walk-through:</h2>

<p align="center">
Step 1 – Log into Windows Server 2022<br/><br/>
Start the virtual machine and log in using the Administrator account credentials created during from the previous setup: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%201.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 2 – Rename the Server<br/><br/>
Open Server Manager and navigate to Local Server. Click on the current computer name, select Change, and rename the server to CA-DC-01. Restart the server to apply the changes: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%202.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br />
Step 3 – Install Active Directory Domain Services<br/><br/>
In Server Manager, click Manage → Add Roles and Features. Proceed through the wizard, select Active Directory Domain Services, add required features, and complete the installation: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%203.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br />
Step 4 – Begin Domain Controller Promotion<br/><br/>
Once installation is complete, click the Notifications flag in Server Manager and select Promote this server to a domain controller to begin configuration: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%204.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br />
Step 5 – Create a New Forest<br/><br/>
Choose Add a new forest and enter your domain name (e.g., Myforest.com). This will create a new Active Directory environment: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%205.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br />
Step 6 – Configure Domain Controller Settings<br/><br/>
Set a Directory Services Restore Mode (DSRM) password. Leave the default settings for domain and forest functional levels, then continue through the setup: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%206.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br />
Step 7 – Install and Promote the Domain Controller<br/><br/>
Proceed through the remaining configuration steps and click Install: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%207.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 8 – Wait for Server Restart<br/><br/>
The system will automatically restart after promotion. Allow the server time to apply all configurations and complete setup: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%208.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 9 – Verify Domain Configuration<br/><br/>
After logging back in, open Command Prompt and run commands such as whoami and systeminfo to confirm the server is part of the new domain and functioning as a Domain Controller: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%209(fix).png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 10 – Confirm Active Directory Installation<br/><br/>
Open Active Directory Users and Computers from Server Manager and verify that your domain (Myforest.com) is present and accessible: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%2010.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 11 – Shut Down the Virtual Machine<br/><br/>
Once verification is complete, safely shut down the virtual machine from VirtualBox: <br/>
<img src="https://github.com/royalexvo/HelpDesk-Home-Lab-Active-Directory-Setup-Domain-Controller-Promotion-Windows-Server-2022-/blob/main/Step%2011.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>
