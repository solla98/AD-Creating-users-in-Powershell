 <p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>AD-Creating Users in Powershell</h1>
This section demonstrates creating multiple random user accounts in Active Directory using PowerShell scripts.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 

## Table of Contents
- [Setup Remote Desktop for non-administrative users on Client-1](#setup-remote-desktop-for-non-administrative-users-on-client-1)
- [Create users](#create-users)


<h2>##Setup Remote Desktop for non-administrative users on Client-1</h2>

<p>
<img width="1452" height="775" alt="image" src="https://github.com/user-attachments/assets/4a3fe261-39cf-48fb-abe3-51e78a39f345" />
<img width="1455" height="780" alt="image" src="https://github.com/user-attachments/assets/bd602576-40cf-4c9a-916a-751d4687d654" />
<img width="1454" height="780" alt="image" src="https://github.com/user-attachments/assets/b351450f-ad0d-4acb-80a7-6d3b82f3c1d1" />



</p>
<p>
Authenticated on Client-1 using mydomain.com\jane_admin. 
  
Accessed System Properties, enabled Remote Desktop, and granted Domain Users permission to connect, allowing standard domain users to log in remotely.

Steps : 

1.Log into Client-1 as mydomain.com\jane_admin.

2.Open System Properties.

3.Click Remote Desktop.

4.Enable access and add the Domain Users group to allow non-admin users to connect via Remote Desktop.
</p>
<br />

<h2>##Create users</h2>

<p>
<img width="1455" height="778" alt="image" src="https://github.com/user-attachments/assets/9133ad95-f57e-4f43-8fab-9f335745981d" />
<img width="1450" height="775" alt="image" src="https://github.com/user-attachments/assets/358b11bc-a5f9-4b44-ad36-9fcdaaa2af51" />
<img width="810" height="737" alt="image" src="https://github.com/user-attachments/assets/56124c02-7ec6-46c3-906f-cd661dfc6b28" />
<img width="1454" height="781" alt="image" src="https://github.com/user-attachments/assets/7dc87867-1c46-466f-bb53-d223426c4d73" />


</p>
<p>
Authenticated on DC-1 using jane_admin, launched PowerShell ISE with administrative privileges, created a new script file, pasted the script contents, executed the script, and verified the successful creation of user accounts

Steps:

1.Log into DC-1 as jane_admin.

2.Launch PowerShell ISE as an administrator.

3.Create a new script file and paste the script contents.

4.Run the script.

5.Observe the automatic creation of domain user accounts.
</p>
<br />

<p>
<img width="1455" height="777" alt="image" src="https://github.com/user-attachments/assets/dff65280-4090-471c-a4b0-8ea731efe010" />


</p>
<p>
Launch Active Directory Users and Computers (ADUC) on DC-1 and confirm that all accounts created via the script are correctly placed within the _EMPLOYEES Organizational Unit
</p>
<br />


