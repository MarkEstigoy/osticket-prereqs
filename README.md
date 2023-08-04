# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/38k39am.jpg" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- MySQL

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Installation Steps</h2>
</p>
<br />

First step is too create your Azure research group. Name it RG-OsTicket
</p>
<br />

<p>
<img src="https://i.ibb.co/h7hrQ34/step1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next step is too create your VM, this is where we will install OS-Ticket 
</p>
<br />

<p>
<img src="https://i.ibb.co/hFPcND0/step1-2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Remote desktop into the VM you've just created
</p>
<br />

<p>
<img src="https://i.ibb.co/gdXrSLq/step1-3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once your in the VM, use this link too access the installation files (https://docs.google.com/document/d/12QH7yrsaiUfYNOgZK7KgTSZQSJ-HYTSVcGFildWMRig/edit)
</p>
<br />
<img src="https://i.ibb.co/ZYTmmtw/step1-4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

</p>
<br />
Here are the installation files (https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)
</p>
<br />
<img src="https://i.ibb.co/pPPsb1n/step1-5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Next step is too enable ISS in Windows WITH CGI and Common HTTPS Features, to do this go too Programs and Features and select the option "Turn Windows features on or off"
</p>
<br />
<img src="https://i.ibb.co/LS5NJ12/step1-6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once thats complete, go into "Internet Information Services" tab then into "World Wide Web Services" then into "Application Development Feautures" then lastly checkmark "CGI" to enable it.
</p>
<br />
<img src="https://i.ibb.co/VC3D5fh/step1-7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/jMjfJ1F/step1-8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Next step is too checkmark all of the options for "Common HTTP Features", you can find this tab under the same tab of "World Wide Web Services"
</p>
<br />

<img src="https://i.ibb.co/jZ8hfvP/step1-9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once we've prepped the VM for installation, we can go ahead and install PHP Manager. (PHPManagerForIIS_V1.5.0.msi) (https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link) 
</p>
<br />
<img src="https://i.ibb.co/kQvrkTm/step2-1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/y00LCMg/step2-2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/q1nvDQJ/step2-3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Next install the Rewrite Module (rewrite_amd64_en-US.msi) (https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)
</p>
<br />
<img src="https://i.ibb.co/F6qwmWR/step2-4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/tHYX9SJ/step2-5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Next step is too create a PHP folder inside the windows (C:)DRIVE
</p>
<br />
<img src="https://i.ibb.co/4VgNYCZ/step2-6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Download PHP from the installation folder (https://drive.google.com/file/d/1snNMtLdCOpMtkCyD4mvl9yOOmvVIp9fP/view?usp=share_link) (php-7.3.8-nts-Win32-VC15-x86.zip)
</p>
<br />
<img src="https://i.ibb.co/JqRrzBb/step2-7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once that download is complete, you can find the file under "Downloads". Extract all the contents of the file and place them under the PHP folder we've created in (C:) Drive
</p>
<br />
<img src="https://i.ibb.co/rH16Q77/step2-8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/dPyCzX7/step2-9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/5L12bh8/step3-0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Next file too download and install is VC_redist.x86.exe (https://drive.google.com/file/d/1s1OsGF3-ioO0_9LYizPRiVuIkb3lFJgH/view?usp=share_link) 
<img src="https://i.ibb.co/CwVPrnx/step3-1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
You can find the file under "Downloads", open it up and press "Install"
</p>
<br />
<img src="https://i.ibb.co/GTkR5ft/step3-2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Next step is download "MySQL"
</p>
<br />
<img src="https://i.ibb.co/TchykbR/step3-3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once its done, open it up and click next 
</p>
<br />
<img src="https://i.ibb.co/p13m3zN/step3-4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
On the setup options you will want too choose "Typical", and "Standard Configuration" 
</p>
<br />
<img src="https://i.ibb.co/Trf0Kmt/step3-5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/XVgJnDC/step3-6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/DQ9CSLC/step3-7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Enter a password (NOTE- Please be sure too write down this password or memorize it, you will need this too login into MySQL later)
</p>
<br />
<img src="https://i.ibb.co/hym736L/step3-8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once all that is completed, press "Execute"
</p>
<br />
<img src="https://i.ibb.co/1fZjRhr/step3-9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Now we have option too run "ISS", type it in the search tab and open it as an administrator. "Run as Administrator" option
</p>
<br />
<img src="https://i.ibb.co/vwWbTnV/step4-0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once your in the ISS app, we will want too register a new PHP. To do this select "PHP Manager" and "Register new PHP version"
</p>
<br />
<img src="https://i.ibb.co/410TxPs/step4-1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/qMmxhgV/step4-2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Go into Windows C: drive and select the "PHP" folder
</p>
<br />
<img src="https://i.ibb.co/BtdL2Rn/step4-3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Select "php-cgi" and press OK afterwards
</p>
<br />
<img src="https://i.ibb.co/hHs7vjv/step4-4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/WfVGyGT/step4-5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
We have now registered PHP
</p>
<br />
<img src="https://i.ibb.co/ckbfmTj/step4-6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Make sure too restart the web server 
</p>
<br />
<img src="https://i.ibb.co/WFLpDs5/step4-7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Now we can download OS-Ticket, you can find the download link in the installation files (https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)
</p>
<br />
<img src="https://i.ibb.co/f1R30K3/step4-8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once you've downloaded OS-Ticket, you will want too drop the "upload" folder into "inetpub" into "wwwroot" (Windows C: > inetpub > wwwroot) 
</p>
<br />
<img src="https://i.ibb.co/cyCDbzC/step5-0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/D1PDhKs/step5-1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/GCwJL0Q/step5-2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/cg4D5mk/step5-3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once the upload folder has been downloaded, RENAME it into OS-Ticket
</p>
<br />
<img src="https://i.ibb.co/B6TZkJ4/step5-4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Restart the VM. You can now find OSticket, select it and press "Browse *:80 (http)" too open up the website 
</p>
<br />
<img src="https://i.ibb.co/FKB3rLM/step5-5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/mFL9V1g/step5-6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/f4MKQCc/step5-7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
The next step is too enable some of the options in our OSTicket 
</p>
<br />
<img src="https://i.ibb.co/kMHMxvz/step5-8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
To do this, go back into ISS > PHP Manager and select "Enable or disable an extension" 
</p>
<br />
<img src="https://i.ibb.co/WtLvJzb/step5-9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/ct2XVpq/step6-0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Enable: (php_imap.dll) (php_intll.dll) (php_opcache.dll) , Refresh OSticket afterwards
</p>
<br />
<img src="https://i.ibb.co/Kr3hYBL/step6-1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/y4Wmdbn/step6-2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
The extensions should now have a green check mark 
</p>
<br />
<img src="https://i.ibb.co/2vJcydT/step6-3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
The next thing we will want too do is rename "ost-sampleconfig.php" into "ost-config.php". We can find ost-sampleconfig.php in the Windows C: > inetpub > wwwroot 
</p>
<br />
<img src="https://i.ibb.co/dfF6rdr/step6-4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/kyvGXnj/step6-5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Next we will want too give everyone permission too manipulate the file, too start this right click on "ost-config" and select properties
</p>
<br />
<img src="https://i.ibb.co/NjDRZXy/step6-6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Now go into Security > Advanced and press "Disable inheritance".
</p>
<br />
<img src="https://i.ibb.co/QcrdNbL/step6-7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Select "Remove all inherited permissions from this object"
</p>
<br />
<img src="https://i.ibb.co/CHNytpd/step6-8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once thats complete, we can now edit the permissions. Press "Select a principal" and type in "Everyone" 
</p>
<br />
<img src="https://i.ibb.co/5YBL41b/step6-9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/T11yX2w/step7-0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Select all for "Basic Permissions" and hit apply/OK afterwards 
</p>
<br />
<img src="https://i.ibb.co/TPrfbcW/step7-1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/DfKwKhB/step7-2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once thats completed, we will want too set up our Help Desk. Click continue on osTicket 
</p>
<br />
<img src="https://i.ibb.co/GptXSJ5/step7-3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Fill in the empty slots (Please make sure you remember username/password)
</p>
<br />
<img src="https://i.ibb.co/KFLwqr3/step7-4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Next step is too download HeidiSQL (https://docs.google.com/document/d/1WovrX2DaS9xkfaSr4LXyB4YnnWpXIgPCMMbbfgHmGVw/edit)
</p>
<br />
<img src="https://i.ibb.co/c88k507/step7-5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Continue pressing next on default settings
</p>
<br />
<img src="https://i.ibb.co/WBXwFhK/step7-6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/0DbgJ4s/step7-7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Next step, we will want too set up a new connection. Once HeidiSQL launches, press "New" then sign in using the username and password we have typed in when we first installed MySQL 
</p>
<br />
<img src="https://i.ibb.co/5RN1bt5/step7-8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Once we are in, we want too create a new database for OSticket. Right click on Unamed > Create new > Database 
</p>
<br />
<img src="https://i.ibb.co/T1wsq6m/step7-9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/gSXfYmS/step8-0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
After clicking "Database" type in "osTicket" too create it 
</p>
<br />
<img src="https://i.ibb.co/zZzNXBz/step8-1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
After creating osTicket in HeidiSQL, go back into osTicket installer and fill in the blanks for "Database Settings". Click "Install Now" once everything is typed 
</p>
<br />
<img src="https://i.ibb.co/WD9wQ7L/step8-2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Congratulations! You've now installed OsTicket! 
</p>
<br />
<img src="https://i.ibb.co/NKk9x8t/step8-3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Now we are going too do a little bit of clean up, go in Windows (C:) > inetpub > wwwroot > OsTicket and DELETE the "setup" folder
</p>
<br />
<img src="https://i.ibb.co/mqHB2fD/step8-4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Now we are going too change the permissions. Go into ost-config > properties and select "Everyone" and press Advanced too edit the permissions. 
</p>
<br />
<img src="https://i.ibb.co/2jSdkbq/step8-5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/LxXmzgF/step8-6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
Uncheck all the boxes except for "Read & execute", hit Apply and OK afterwards
</p>
<br />
<img src="https://i.ibb.co/MhPR2Mj/step8-7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.ibb.co/vZbRJk6/step8-8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />











