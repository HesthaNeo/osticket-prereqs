<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable Internet Information Services (IIS) with CGI (Common Gateway Interface)
- Install Web Platform Installer
- Install C++ Redistributable
- Install MySQL and Setup Username and Password
- Configure Permissions and Install osTicket

<h2>Installation Steps</h2>
<p>
<h1>Step 1: Enable Internet Information Services (IIS) with CGI (Common Gateway Interface)</h1>
</p>
<p>
- First, we open Control Panel, go to Programs and Features, and click Turn Windows Features on or off. From there we scroll down to find IIS, and enable it.
<p>
<img src="https://i.imgur.com/1auhZ9x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
- The next thing was to expand the IIS section, find Application Development Features, and enable the CGI as well.
<p> 
<p>
<img src="https://i.imgur.com/TMm3m0Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<h1>Step 2: Install Web Platform Installer</h1>
</p>
<p>
- In this step, we will install the Web Platform Installer. To do that, we must first download and install the PHP Manager for IIS.
</p>
<p>
<img src="https://i.imgur.com/dvRGYh4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/zcVEfvA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Next, was to download and install the rewrite module.
</p>
<p>
<img src="https://i.imgur.com/IHmjB4G.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/cvy9y6B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/B05X8xj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- After installing the rewrite module, we needed to create the directory C:\PHP, in order to install the PHP zip file that we were required to download.
<p/>
<p>
<img src="https://i.imgur.com/e30wr5m.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/tFEJ4f6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<h1><p> Step 3: Install C++ Redistributable</h1>
</p>
<p>
- Next is to install the C++ Redistributable file for the installation.
</p>
<p>
<img src="https://i.imgur.com/JudjfNP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/k1BomJx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/9QXJKrT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h1><p> Step 4: Install MySQL and Setup Username and Password</h1>
</p>
<p> 
- For this step, we will install my SQL for our database server management.
</p>
<p>
<img src="https://i.imgur.com/4htBXSF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- We used Typical Setup for this installation.
<p>
<img src="https://i.imgur.com/1kipAj6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/HHgDG3I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- After the installation, we make sure to launch the Configuration Wizard.
<p>
<img src="https://i.imgur.com/G6BUp9i.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Use the Standard Configuration and install.
<p>
<img src="https://i.imgur.com/0ZrRzsS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/H6G2VHy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h1><p> Step 5: Configure Permissions and Install osTicket</h1>
</p>
<p> 
- In this step, in order to configure the permissions and install osTicket, we begin by opening IIS as an admin. After doing that, we register PHP from within IIS.
</p>
<p>
<img src="https://i.imgur.com/twEf0iH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
- Registering PHP in IIS. (Restart the Server)
</p>
<p>
<img src="https://i.imgur.com/jXujTa2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/zXI8GbD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 
<p> 
- Next was to install osTicket that we downloaded previously and to extract the upload folder to c:\inetpub\wwwroot. (Restart the Server)
</p>
<p>
<img src="https://i.imgur.com/2gevzDj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
- Next, in IIS, we go to Sites, Default, osTicket. On the right side, we click "Browse *:80 (http)"
<p>
<img src="https://i.imgur.com/3asSOdu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/vAB8JuZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
- Since some of the extensions were still not enabled, we went back to IIS and clicked on Sites, Default, osTicket. From there we clicked on PHP Manager where we clicked Enable or disable extension.
</p>
<p>
<img src="https://i.imgur.com/YlnyHAk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
- We made sure to enable php_imap.dll, php_intl.dll, and php_opcache.dll.
</p>
<p>
<img src="https://i.imgur.com/15NESF5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
- After refreshing the osTicket site in the browser, we can see that the extensions we selected were enabled.
</p>
<p>
<img src="https://i.imgur.com/iggkGzO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Next was to rename the configuration file for PHP from: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php, to: C:\inetpub\wwwroot\osTicket\include\ost-config.php
</p>
<p>
<img src="https://i.imgur.com/hKieodf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/T6PmTIf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- We assigned permissions for ost-config.php, which included Disable Inheritance, and then adding New Permissions to Everyone with All permissions.
</p>
<p>
<img src="https://i.imgur.com/sap6H01.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- From there, we can continue to setting up osTicket in our web browser.
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- In order to continue with the setup of osTicket, we need to download and install Heidi SQL.
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- After installation, we created a new session, connected to the session, and inside Heidi SQL, created a database called "osTicket".
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Once completed, we head back to our web browser to continue setting up osTicket with the apppropriate credentials.
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- After this, we can click install now, and osTicket has been successfully installed. We can browse to our osTicket help desk login page, and see our fully functioning ticketing system.
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
