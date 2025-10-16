<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a virtual machine
- Configure system prerequisites
- Install osTicket files
- Set up IIS and PHP
- Verify installation success

<h2>Installation Steps</h2>

<p>
<img width="713" height="743" alt="Createvituralmachine" src="https://github.com/user-attachments/assets/1b2c7243-203d-470d-8d46-3631e022b289" />
</p>
<p>
Create the Azure virtual machine and allocate CPU, memory, and disk before connecting.
</p>
<br />

<p>
<img width="704" height="638" alt="Screenshot 2025-09-25 at 9 30 01 PM" src="https://github.com/user-attachments/assets/da779a04-4434-4958-bd4f-3f58cd0a9ae6" />
</p>
<p>
Use Remote Desktop Protocol (RDP) to connect to the Windows VM with admin credentials.
</p>
<br />

<p>
<img width="661" height="228" alt="Screenshot 2025-09-25 at 9 37 48 PM" src="https://github.com/user-attachments/assets/a224a09e-4b38-4144-8ef7-5b58bdbc5b5b" />
</p>
<p>
Open Server Manager or Control Panel to install IIS and required Windows features.
</p>
<br />

<p>
<img width="426" height="464" alt="Screenshot 2025-09-25 at 9 39 33 PM" src="https://github.com/user-attachments/assets/c09d43fc-4b6c-4f06-b65a-a5ef6aedcaf2" />
</p>
<p>
Enable CGI and IIS URL Rewrite, then restart IIS to apply feature changes.
</p>
<br />

<p>
<img width="720" height="825" alt="Screenshot 2025-09-25 at 9 43 34 PM" src="https://github.com/user-attachments/assets/d285221c-83bb-461e-81af-595b5202ce49" />
</p>
<p>
Install PHP for Windows (use Web Platform Installer or manual PHP build) and verify PHP works with IIS.
</p>
<br />

<p>
<img width="1122" height="594" alt="Screenshot 2025-09-25 at 9 45 01 PM" src="https://github.com/user-attachments/assets/dda9986d-639c-4cfd-a0ff-268bc96a2028" />
</p>
<p>
Install MySQL or MariaDB on the Windows server and prepare for database creation.
</p>
<br />

<p>
<img width="1061" height="594" alt="Screenshot 2025-09-25 at 9 50 19 PM" src="https://github.com/user-attachments/assets/319367c3-bce4-4197-91c4-28577472b961" />
</p>
<p>
Run the MySQL secure setup and create a strong root password and initial users.
</p>
<br />

<p>
<img width="720" height="829" alt="Screenshot 2025-09-25 at 9 54 28 PM" src="https://github.com/user-attachments/assets/c0f2736f-65aa-40fb-9a1e-2b2b858fe6b4" />
</p>
<p>
Install required PHP extensions (mysqli, mbstring, gd, json) and confirm the PHP version in IIS.
</p>
<br />

<p>
<img width="1124" height="590" alt="Screenshot 2025-09-25 at 9 57 19 PM" src="https://github.com/user-attachments/assets/29e07c22-f973-491e-9536-94c17e8ed007" />
</p>
<p>
Create a database and dedicated database user for osTicket with appropriate privileges.
</p>
<br />

<p>
<img width="1119" height="590" alt="Screenshot 2025-09-25 at 9 59 06 PM" src="https://github.com/user-attachments/assets/4ddb65d2-8c65-4cb3-aeb8-eef5f5cc7fa8" />
</p>
<p>
Download and extract the osTicket package to the IIS site folder (e.g., `C:\inetpub\wwwroot\osticket`).
</p>
<br />

<p>
<img width="608" height="546" alt="Screenshot 2025-09-25 at 10 00 53 PM" src="https://github.com/user-attachments/assets/96d7bb20-67e3-48ea-bbb3-b44209cd2e1d" />
</p>
<p>
Set NTFS permissions for the IIS App Pool identity (or `IIS_IUSRS`) on upload and include folders.
</p>
<br />

<p>
<img width="1004" height="451" alt="Screenshot 2025-09-25 at 10 02 07 PM" src="https://github.com/user-attachments/assets/480c94e8-f437-4ad9-9ba1-374ac566e918" />
</p>
<p>
Create an IIS site or application for osTicket and set the site bindings for HTTP/HTTPS.
</p>
<br />

<p>
<img width="730" height="302" alt="Screenshot 2025-09-25 at 10 03 25 PM" src="https://github.com/user-attachments/assets/59211040-2672-4507-b9dd-1094a5dd25f6" />
</p>
<p>
Open the osTicket installer URL in a browser to access the web-based setup page.
</p>
<br />

<p>
<img width="902" height="389" alt="Screenshot 2025-09-25 at 10 04 35 PM" src="https://github.com/user-attachments/assets/56f248b8-1ee3-4714-ba64-e1eb97109d01" />
</p>
<p>
Review the installer system requirements and confirm all PHP extensions and permissions.
</p>
<br />

<p>
<img width="498" height="379" alt="Screenshot 2025-09-25 at 10 05 35 PM" src="https://github.com/user-attachments/assets/b38bcc36-0f0c-447e-96ea-de0eeb62c25c" />
</p>
<p>
Enter database host, database name, username, and password in the installer form.
</p>
<br />

<p>
<img width="500" height="379" alt="Screenshot 2025-09-25 at 10 06 15 PM" src="https://github.com/user-attachments/assets/d87742dc-25d8-4b49-9f23-94ca96ae22b1" />
</p>
<p>
Provide the admin account details (email, username, and password) to create the administrator account.
</p>
<br />

<p>
<img width="771" height="667" alt="Screenshot 2025-09-25 at 10 12 18 PM" src="https://github.com/user-attachments/assets/2725a6ee-e93f-4314-b8a1-f73b60ddfe7a" />
</p>
<p>
Confirm the installer completes and that osTicket database tables are created successfully.
</p>
<br />

<p>
<img width="717" height="860" alt="Screenshot 2025-09-25 at 10 13 59 PM" src="https://github.com/user-attachments/assets/32f159a4-3ec9-4a3a-81d5-b23776c78cd9" />
</p>
<p>
After install, follow instructions to remove or secure the `setup` directory to prevent reuse.
</p>
<br />

<p>
<img width="1014" height="399" alt="Screenshot 2025-09-25 at 10 16 33 PM" src="https://github.com/user-attachments/assets/dc13d701-5991-4b8b-b884-8ea2f59d42c9" />
</p>
<p>
Log in to the osTicket admin panel to verify admin access and initial dashboard view.
</p>
<br />

<p>
<img width="597" height="757" alt="Screenshot 2025-09-25 at 10 24 37 PM" src="https://github.com/user-attachments/assets/a8625a86-cd05-4b17-a622-61767b48bcb8" />
</p>
<p>
Check the agent dashboard to confirm queues, recent tickets, and system notices display correctly.
</p>
<br />

<p>
<img width="509" height="136" alt="Screenshot 2025-09-25 at 10 25 44 PM" src="https://github.com/user-attachments/assets/04b6d8ab-f93b-423a-83d7-1ff9d9d61760" />
</p>
<p>
Configure organization settings such as name, default email, and contact information.
</p>
<br />

<p>
<img width="404" height="421" alt="Screenshot 2025-09-25 at 10 26 46 PM" src="https://github.com/user-attachments/assets/2e53f48c-fe9e-4f36-b202-2081e60ec575" />
</p>
<p>
Set up email routing: incoming (POP/IMAP) or piping, then test message delivery.
</p>
<br />

<p>
<img width="1440" height="858" alt="Screenshot 2025-09-25 at 10 28 33 PM" src="https://github.com/user-attachments/assets/9c25f8b8-4280-434c-acf4-978ce6ce015f" />
</p>
<p>
Create help topics, forms, and email templates used by customers in the portal.
</p>
<br />

<p>
<img width="719" height="851" alt="Screenshot 2025-09-25 at 10 37 23 PM" src="https://github.com/user-attachments/assets/47e9552b-97ae-4254-a544-4ae490f7d04b" />
</p>
<p>
Create queues and departments, and assign agents or groups for testing.
</p>
<br />

<p>
<img width="705" height="738" alt="Screenshot 2025-09-25 at 10 38 26 PM" src="https://github.com/user-attachments/assets/7fa4ea38-d65e-4d66-9d57-e865a1128549" />
</p>
<p>
Submit a test ticket with an attachment to verify uploads and visibility.
</p>
<br />

<p>
<img width="622" height="599" alt="Screenshot 2025-09-25 at 10 42 29 PM" src="https://github.com/user-attachments/assets/65e97706-bbba-4e86-9f88-eb3ee0e7567d" />
</p>
<p>
Open a sample ticket and confirm status, priority, and internal notes function correctly.
</p>
<br />

<p>
<img width="765" height="516" alt="Screenshot 2025-09-25 at 10 44 03 PM" src="https://github.com/user-attachments/assets/e86f174a-8047-4dd3-8c4e-07efb88aee35" />
</p>
<p>
Configure SLA rules, autoresponders, and canned replies for common scenarios.
</p>
<br />

<p>
<img width="910" height="588" alt="Screenshot 2025-09-25 at 10 45 48 PM" src="https://github.com/user-attachments/assets/ba38a08a-927f-4388-acb6-c95fbbb23ab0" />
</p>
<p>
Check server logs and osTicket logs for any errors or permission issues.
</p>
<br />

<p>
<img width="759" height="516" alt="Screenshot 2025-09-25 at 10 46 01 PM" src="https://github.com/user-attachments/assets/f2416ca2-00f9-43fc-a3a5-48650696aab6" />
</p>
<p>
Back up the database and configuration files to preserve the working state.
</p>
<br />

<p>
<img width="1031" height="712" alt="Screenshot 2025-09-25 at 10 51 53 PM" src="https://github.com/user-attachments/assets/dc6cae41-a47d-4801-a2b3-3e829bdde3a3" />
</p>
<p>
Verify Azure network security group and Windows firewall rules allow HTTP/HTTPS.
</p>
<br />

<p>
<img width="686" height="483" alt="Screenshot 2025-09-25 at 10 53 22 PM" src="https://github.com/user-attachments/assets/b985114f-5bf4-4319-a803-e1551c406a50" />
</p>
<p>
Optionally configure SSL/TLS (for example use certbot on a reverse proxy or a Windows certificate) and require HTTPS.
</p>
<br />

<p>
<img width="565" height="509" alt="Screenshot 2025-09-25 at 10 54 42 PM" src="https://github.com/user-attachments/assets/0c0d68aa-0e6e-44f5-8a1c-96c0604be870" />
</p>
<p>
Confirm scheduled tasks (if used) and background jobs are configured and running.
</p>
<br />

<p>
<img width="525" height="329" alt="Screenshot 2025-09-25 at 10 55 26 PM" src="https://github.com/user-attachments/assets/d22c02a8-558a-4fb6-9869-49e56f7d832d" />
</p>
<p>
Double-check NTFS permissions on osTicket files and upload directories.
</p>
<br />

<p>
<img width="684" height="740" alt="Screenshot 2025-09-25 at 10 56 30 PM" src="https://github.com/user-attachments/assets/3d0c4c19-1aba-4791-842a-22113ad3eac1" />
</p>
<p>
Test the customer portal by submitting a ticket and confirm email notifications.
</p>
<br />

<p>
<img width="721" height="856" alt="Screenshot 2025-09-25 at 10 58 26 PM" src="https://github.com/user-attachments/assets/70a4c5c9-4509-48e7-b054-48c7ecb24e98" />
</p>
<p>
Reply to the test ticket from an agent account and verify the user receives the response.
</p>
<br />

<p>
<img width="713" height="401" alt="Screenshot 2025-09-25 at 10 59 32 PM" src="https://github.com/user-attachments/assets/a814c321-4135-4380-8dd3-3fce33c0f44f" />
</p>
<p>
Complete final checks: backups, monitoring, and secure admin credential storage.
</p>
<br />
