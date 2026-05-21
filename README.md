<h1>Active Directory Home Lab</h1>

<h2>Description</h2>
This project documents the setup of a basic Active Directory home lab using Oracle VirtualBox, Windows Server 2019, and Windows 10. The lab demonstrates domain controller configuration, DHCP, DNS, NAT, PowerShell user automation, and domain-joined client administration
<br />


<h2>Technologies Used</h2>

- <b>Active Directory Domain Services (AD DS)</b>
- <b>PowerShell</b>
- <b>DHCP and DNS</b> 
<h2>Environments Used </h2>

- <b>VMware Fusion</b>
- <b>Windows 11</b> 

## Skills Practiced
- Active Directory administration
- User and group management
- PowerShell scripting
- Windows Server configuration
- Networking fundamentals
- DHCP and DNS configuration
- System troubleshooting
- Domain administration

<h2>Lab Walk-Through:</h2>

<p align="center">
Check the Windows 11 network: <br/>
<img src="https://i.imgur.com/1U3dpbm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h3 align="center">Step 3: Set the Preferred DNS Server</h3>

<p align="center">
  <img src="https://i.imgur.com/xVuBVaR.png" width="80%" alt="Preferred DNS settings"/>
</p>

<p>
<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I opened the Windows 11 Ethernet settings and manually set the Preferred DNS server to <code>172.16.23.2</code>.
This allows the Windows 11 client to use the correct DNS server before joining the Active Directory domain.
</p>
</p>

<p>
This allows the Windows 11 client to use the correct DNS server before joining the Active Directory domain.
</p>
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
