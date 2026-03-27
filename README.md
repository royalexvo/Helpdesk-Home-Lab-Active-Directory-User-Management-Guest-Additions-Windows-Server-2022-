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
Start the virtual machine and log in using the Administrator account credentials created in the previous lab: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%201.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 2 – Install VirtualBox Guest Additions<br/><br/>
Insert the Guest Additions CD from the VirtualBox menu and run the installer. Follow the prompts (Next → Install) and reboot the machine when prompted: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%202.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br />
Step 3 – Configure Shared Folder<br/><br/>
Create a shared folder on the host machine and map it in VirtualBox settings. Enable Auto-mount and Make Permanent to allow seamless file transfer between host and VM: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%202.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br />
Step 4 – Test File Transfer<br/><br/>
Copy a file (e.g., image) from the host system and paste it into the shared folder inside the VM to verify Guest Additions is working correctly: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%204.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br />
Step 5 – Open Active Directory Users and Computers<br/><br/>
Launch Active Directory Users and Computers (ADUC) and expand the domain to access organizational units such as Users: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%205.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br />
Step 6 – Create a New User Account<br/><br/>
Right-click the Users container → New → User. Enter user details (e.g., John Doe), assign a password, and complete the setup: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%206.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br />
Step 7 – Verify User Creation<br/><br/>
Confirm the new user appears in the Users container within Active Directory: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%207.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 8 – Modify User Properties<br/><br/>
View/edit user details such as: Address and location, Phone number, Department and job title, and Manager/reporting structure: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%208.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 9 – Manage User Account Settings<br/><br/>
Use right-click options to: Reset password, Disable or enable account, Unlock account, or Configure logon hours: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%209.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 10 – Configure Logon Hours<br/><br/>
Restrict when a user can log in by selecting allowed days and times. This can fully block or limit access based on business requirements: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%2010.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 11 – Verify User via Command Line<br/><br/>
Use the following command to check account details: net user "John Doe" /domain. This displays password info, group membership, and account status: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%2011.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 12 – Create Additional Users<br/><br/>
Repeat the process to create additional accounts (e.g., Kevin) for future labs and testing scenarios: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%2012.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
<br/>
Step 13 – Lab Completion<br/><br/>
This lab focuses on foundational Active Directory tasks such as user creation and basic account management. Future labs will involve joining client machines (Windows 11) to the domain and expanding functionality: <br/>
<img src="https://github.com/royalexvo/Helpdesk-Home-Lab-Active-Directory-User-Management-Guest-Additions-Windows-Server-2022-/blob/main/Step%2013.png?raw=true" height="80%" width="80%" alt="Lab Steps"/>
</p>
