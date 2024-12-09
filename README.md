<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>


<p>
  <strong>1. Log into osTicket as an Admin:</strong><br>
  - Start by visiting the Admin Login page: http://localhost/osTicket/scp/login.php<br>
  - Log in with Admin username and password.<br>
  - Once logged in, click on Admin Panel at the top right to see the backend configuration options.
</p>

<p>
  <img src="https://i.imgur.com/ZUIdwVY.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <img src="https://i.imgur.com/2I3IW6Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>2. Configure A New Role:</strong><br>
  - Click on the Agents tab and select Roles.<br>
  - For Name, type Supreme Admin for the new role we'll be creating.<br>
  - Before clicking on Add Role, click on the Permissions tab next to Definition.<br>
  - We are going to allow this role to have all permissions. To do so, select all available options under Tickets, Tasks and Knowledgebase. Each option should be checked.<br>
  - Once all options have been checked, click on Add Role at the bottom.
</p>

<br>

<p>
  <img src="https://i.imgur.com/C56v4Ud.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <img src="https://i.imgur.com/mA9GnpQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>3. Configure A New Department:</strong><br>
  - Click on the Agents tab and select Departments.<br>
  - Click on Add New Department.<br>
  - For Parent, select Support from the drop-down options.<br>
  - For Name, type SysAdmins for the new department we'll be creating.<br>
  - Click on Create Dept at the bottom.
</p>

<p>
  <img src="https://i.imgur.com/jm5fOee.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>4. Configure A New Team:</strong><br>
  - Click on the Agents tab and select Teams.<br>
  - Click on Add New Team.<br>
  - For Name, type Online Banking for the new team we'll be creating.<br>
  - Click on Create Team at the bottom.
</p>

<p>
  <img src="https://i.imgur.com/gWL043m.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>5. Configure A New Agent:</strong><br>
  - Click on the Agents tab and select Agents.<br>
  - Click on Add New Agent.<br>
  - On the Account tab, enter a name, email address and username.<br>
  - On the Access tab, select Support/SysAdmins as the department and select Supreme Admin as the role from the drop-down options.<br>
  - On the Teams tab, select Online Banking as the team from the drop-down options.<br>
  - Click on Create at the bottom.
</p>

<p>
  <img src="https://i.imgur.com/9A23XY2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <img src="https://i.imgur.com/ppycbCY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <img src="https://i.imgur.com/o4hOJNZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>6. Set Agent Password:</strong><br>
  - Click on the Agents tab and select Agents.<br>
  - Click on the Agent you just created.<br>
  - On the Account tab, click on Set Password next to Username.<br>
  - Uncheck the reset email option and enter a password for the agent.<br>
  - Click Update at the bottom.
</p>

<p>
  <img src="https://i.imgur.com/4FD4ocp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>7. Configure A New User:</strong><br>
  - Click on Agent Panel at the top right.<br>
  - Click on the Users tab and select Add User.<br>
  - Enter an email address and full name.<br>
  - Click Add User at the bottom.
</p>

<p>
  <img src="https://i.imgur.com/j1j34uv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <img src="https://i.imgur.com/x83qzwo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>8. Set Up PHP:</strong><br>
  - Create a folder named PHP in the *C:* drive.<br>
  - Extract PHP 7.3.8 from the installation files (php-7.3.8-nts-Win32-VC15-x866.zip) and select C:\PHP folder as the destination.
</p>

<p>
  <img src="https://i.imgur.com/XyuQhzY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br>

<p>
  <strong>9. Install the Visual C++ Redistributable:</strong><br>
  - Download the VC_redist.x86.exe from the installation files.<br>
  - Run the installer and follow the setup wizard to complete the installation.
</p>

<p>
  <img src="https://i.imgur.com/YjepQT2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>10. Install the MySQL database:</strong><br>
  - Download MySQL 5.5.62 (mysql-5.5.62-win32.msi) from the installation files.<br>
  - In the setup wizard, select Typical as the Setup Type and select Launch the MySQL Instance Configuration Wizard after installation to finish.<br>
  - Choose Standard Configuration and set a root password.
</p>

<p>
  <img src="https://i.imgur.com/mhc1JQQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>11. Open IIS Manager:</strong><br>
  - Open and run Internet Information Services (IIS) Manager as an administrator.
</p>

<p>
  <img src="https://i.imgur.com/JsMMz8l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>12. Register PHP with IIS:</strong><br>
  - In IIS Manager, locate and click on PHP Manager.<br>
  - Select Register new PHP version.<br>
  - When prompted, provide the path to the PHP executable file (php-cgi.exe). Navigate to C:\PHP, and select the php-cgi.exe file.<br>
  - Finally, restart the IIS server for the changes to take effect.
</p>

<p>
  <img src="https://i.imgur.com/h1xmoYJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br>

<p>
  <strong>13. Install osTicket v1.15.8:</strong><br>
  - Download osTicket v1.15.8 from the Installation Files folder.<br>
  - Extract the contents and copy the upload folder to C:\inetpub\wwwroot.<br>
  - Inside C:\inetpub\wwwroot, rename the upload folder to osTicket.<br>
  - Finally, restart the IIS server for the changes to take effect.
</p>

<p>
  <img src="https://i.imgur.com/AiyOKaL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>14. Access osTicket through IIS:</strong><br>
  - In IIS Manager, navigate to Sites -> Default by clicking the drop-down arrows on the left.<br>
  - Select the osTicket folder.
  - On the right, click *Browse :80* to access osTicket in your web browser.<br>
    <strong>Enable Required PHP Extensions:</strong><br>
    - Go back to IIS Manager and navigate to Sites -> Default -> osTicket once again.<br>
    - Double-click on PHP Manager.<br>
    - At bottom you'll see PHP Extensions. Select Enable or disable an Extension.<br>
    <strong>Enable the following extensions in the disabled list:</strong><br>
    - php_imap.dll<br>
    - php_intl.dll<br>
    - php_opcache.dll
</p>

<p>
  <img src="https://i.imgur.com/F4CNh7Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <img src="https://i.imgur.com/jspFy1N.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>15. Rename the Configuration File and Set Permissions:</strong><br>
  - Open File Explorer and navigate to the following directory: C:\inetpub\wwwroot\osTicket\include.<br>
  - Locate the file ost-sampleconfig.php and rename it to ost-config.php.<br>
  - After renaming the file, right-click on it and select Properties. In the Properties window, go to the Security tab and click on Advanced.<br>
  - Select Disable inheritance at the bottom.
  - Select Remove all inherited permissions from this object.<br>
    <strong>Add new permissions:</strong><br>
    1. Click Add.<br>
    2. Click Select a principal.<br>
    3. Type Everyone in the box and click Check Names.<br>
    4. Click OK.<br>
    5. Make sure Full Control is selected, and all other checkboxes are ticked.<br>
    6. Click Apply and then OK.
</p>

<p>
  <img src="https://i.imgur.com/BG8bn6V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <img src="https://i.imgur.com/8qjGMEH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <img src="https://i.imgur.com/BcbnBYH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br>

<p>
  <strong>16. Complete osTicket Setup in the Browser:</strong><br>
  - In the browser, click Continue on the osTicket setup page.<br>
  - Fill out the required fields on the page, but leave the Database Settings section blank for now; we'll address that shortly. Do not click Install Now yet.<br>
  - Download and install HeidiSQL from the Installation Files.<br>
  - Once HeidiSQL is installed, open the program and create a new session.<br>
  - Make sure the Username is set to root and the Password is root.
</p>

<p>
  <img src="https://i.imgur.com/NkxPGYo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <img src="https://i.imgur.com/hFVBYk6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  <strong>17. Create a New Database in HeidiSQL:</strong><br>
  - In HeidiSQL, right-click on Unnamed on the left panel, select Create New, and then choose Database.<br>
  - Name the new database osTicket.<br>
  - Once the database is created, go back to the osTicket browser setup and enter osTicket as the database name under the MySQL Database section.
</p>

<p>
  <img src="https://i.imgur.com/C1JDtwq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br>

<p>
  <strong>18. Complete the osTicket Setup:</strong><br>
  - The final step is to log in to osTicket via your browser.<br>
  - Congratulations! You have successfully installed and set up osTicket!
</p>

<p>
  <img src="https://i.imgur.com/b5WRFMb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
