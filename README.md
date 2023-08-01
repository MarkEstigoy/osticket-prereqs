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



