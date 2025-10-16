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
Create the virtual machine in Azure with the chosen name, CPU, memory, and disk allocation before starting the installation.
</p>
<br />

<p>
<img width="704" height="638" alt="Screenshot 2025-09-25 at 9 30 01 PM" src="https://github.com/user-attachments/assets/da779a04-4434-4958-bd4f-3f58cd0a9ae6" />
</p>
<p>
Input the VM credentials into Remote Desktop (windows) or Windows App (Mac) to begin the operating system installation.
</p>
<br />

<p>
<img width="661" height="228" alt="Screenshot 2025-09-25 at 9 37 48 PM" src="https://github.com/user-attachments/assets/a224a09e-4b38-4144-8ef7-5b58bdbc5b5b" />
</p>
<p>
Open a terminal session after installation to run commands for system updates and software installation.
</p>
<br />

<p>
<img width="426" height="464" alt="Screenshot 2025-09-25 at 9 39 33 PM" src="https://github.com/user-attachments/assets/c09d43fc-4b6c-4f06-b65a-a5ef6aedcaf2" />
</p>
<p>
Update the package lists and install available security updates so the system is current.
</p>
<br />

<p>
<img width="720" height="825" alt="Screenshot 2025-09-25 at 9 43 34 PM" src="https://github.com/user-attachments/assets/d285221c-83bb-461e-81af-595b5202ce49" />
</p>
<p>
Install the web server (Apache or nginx) and verify the service is active and serving requests.
</p>
<br />

<p>
<img width="1122" height="594" alt="Screenshot 2025-09-25 at 9 45 01 PM" src="https://github.com/user-attachments/assets/dda9986d-639c-4cfd-a0ff-268bc96a2028" />
</p>
<p>
Install the database server (MariaDB or MySQL) and prepare it for osTicket database creation.
</p>
<br />

<p>
<img width="1061" height="594" alt="Screenshot 2025-09-25 at 9 50 19 PM" src="https://github.com/user-attachments/assets/319367c3-bce4-4197-91c4-28577472b961" />
</p>
<p>
Run the database security utility (for example `mysql_secure_installation`) to set passwords and remove default accounts.
</p>
<br />

<p>
<img width="720" height="829" alt="Screenshot 2025-09-25 at 9 54 28 PM" src="https://github.com/user-attachments/assets/c0f2736f-65aa-40fb-9a1e-2b2b858fe6b4" />
</p>
<p>
Install PHP and the required PHP extensions that osTicket depends on, then confirm the PHP version.
</p>
<br />

<p>
<img width="1124" height="590" alt="Screenshot 2025-09-25 at 9 57 19 PM" src="https://github.com/user-attachments/assets/29e07c22-f973-491e-9536-94c17e8ed007" />
</p>
<p>
Create a dedicated database and user for osTicket to use when the installer connects to the database.
</p>
<br />

<p>
<img width="1119" height="590" alt="Screenshot 2025-09-25 at 9 59 06 PM" src="https://github.com/user-attachments/assets/4ddb65d2-8c65-4cb3-aeb8-eef5f5cc7fa8" />
</p>
<p>
Download and extract the osTicket package into the web server document root (for example `/var/www/html/osticket`).
</p>
<br />

<p>
<img width="608" height="546" alt="Screenshot 2025-09-25 at 10 00 53 PM" src="https://github.com/user-attachments/assets/96d7bb20-67e3-48ea-bbb3-b44209cd2e1d" />
</p>
<p>
Set file ownership and permissions so the web server user has the required read and write access.
</p>
<br />

<p>
<img width="1004" height="451" alt="Screenshot 2025-09-25 at 10 02 07 PM" src="https://github.com/user-attachments/assets/480c94e8-f437-4ad9-9ba1-374ac566e918" />
</p>
<p>
Create or enable the web server virtual host for osTicket and enable any required modules, then reload the server.
</p>
<br />

<p>
<img width="730" height="302" alt="Screenshot 2025-09-25 at 10 03 25 PM" src="https://github.com/user-attachments/assets/59211040-2672-4507-b9dd-1094a5dd25f6" />
</p>
<p>
Open the installer URL in a browser to confirm the web installer page is reachable.
</p>
<br />

<p>
<img width="902" height="389" alt="Screenshot 2025-09-25 at 10 04 35 PM" src="https://github.com/user-attachments/assets/56f248b8-1ee3-4714-ba64-e1eb97109d01" />
</p>
<p>
Review the system requirements page and ensure all listed PHP extensions and file permissions are satisfied.
</p>
<br />

<p>
<img width="498" height="3
