<h1>Active Directory Home Lab</h1>

<h2>Description</h2>

<p>
This project documents the setup of a basic Active Directory home lab using VMware Fusion, Windows Server, and Windows 11. 
The lab demonstrates basic networking, DNS configuration, and joining a Windows 11 client machine to an Active Directory domain.
</p>

<h2>Technologies Used</h2>

<ul>
  <li><b>Active Directory Domain Services (AD DS)</b></li>
  <li><b>DNS</b></li>
  <li><b>Windows Server</b></li>
  <li><b>Windows 11</b></li>
</ul>

<h2>Environments Used</h2>

<ul>
  <li><b>VMware Fusion</b></li>
  <li><b>Windows Server</b></li>
  <li><b>Windows 11 Client</b></li>
</ul>

<h2>Skills Practiced</h2>

<ul>
  <li>Active Directory administration</li>
  <li>Windows client configuration</li>
  <li>DNS configuration</li>
  <li>Networking fundamentals</li>
  <li>System troubleshooting</li>
  <li>Domain administration</li>
</ul>

<h2>Lab Walk-Through</h2>

<h3 align="center">Step 1: Start the Lab Environment</h3>

<p align="center">
  <img src="https://i.imgur.com/1U3dpbm.png" width="80%" alt="Lab environment started"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I started the Windows Server and Windows 11 virtual machines in VMware Fusion. 
The Windows Server machine will act as the domain controller, and the Windows 11 machine will act as the client workstation.
</p>

<br />

<h3 align="center">Step 2: Check the Windows 11 Network Settings</h3>

<p align="center">
  <img src="https://i.imgur.com/1U3dpbm.png" width="80%" alt="Windows 11 ipconfig output"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I opened Command Prompt and ran <code>ipconfig /all</code> to check the Windows 11 client network settings. 
The Windows 11 client had the IP address <code>172.16.23.128</code> and the DNS server <code>172.16.23.2</code>.
</p>

<br />

<h3 align="center">Step 3: Set the Preferred DNS Server</h3>

<p align="center">
  <img src="https://i.imgur.com/xVuBVaR.png" width="80%" alt="Preferred DNS settings"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I opened the Windows 11 Ethernet settings and manually set the Preferred DNS server to <code>172.16.23.2</code>. 
This allows the Windows 11 client to use the correct DNS server before joining the Active Directory domain.
</p>

<br />

<h3 align="center">Step 4: Test Connection to the Domain Controller</h3>

<p align="center">
  <img src="YOUR_IMAGE_LINK_HERE" width="80%" alt="Ping test to domain controller"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I used the <code>ping</code> command to test if the Windows 11 client could communicate with the domain controller. 
This confirmed that the client and server were able to communicate on the network.
</p>

<br />

<h3 align="center">Step 5: Open Domain Join Settings</h3>

<p align="center">
  <img src="YOUR_IMAGE_LINK_HERE" width="80%" alt="Domain join settings"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I opened the Windows system settings to prepare the Windows 11 client to join the Active Directory domain.
</p>

<br />

<h3 align="center">Step 6: Join the Windows 11 Client to the Domain</h3>

<p align="center">
  <img src="YOUR_IMAGE_LINK_HERE" width="80%" alt="Join Windows 11 to domain"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I entered the domain name and joined the Windows 11 client to the Active Directory domain using domain administrator credentials.
</p>

<br />

<h3 align="center">Step 7: Restart the Windows 11 Client</h3>

<p align="center">
  <img src="YOUR_IMAGE_LINK_HERE" width="80%" alt="Restart Windows 11 client"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
After joining the domain, I restarted the Windows 11 client so the domain changes could take effect.
</p>

<br />

<h3 align="center">Step 8: Log In With a Domain Account</h3>

<p align="center">
  <img src="YOUR_IMAGE_LINK_HERE" width="80%" alt="Domain account login"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
After the restart, I logged in to the Windows 11 client using a domain user account.
</p>

<br />

<h3 align="center">Step 9: Verify the Computer in Active Directory</h3>

<p align="center">
  <img src="YOUR_IMAGE_LINK_HERE" width="80%" alt="Computer object in Active Directory"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I opened Active Directory Users and Computers on the domain controller and confirmed that the Windows 11 client appeared as a computer object in the domain.
</p>

<br />

<h2>Help Desk Skills Demonstrated</h2>

<ul>
  <li>Checked Windows network configuration</li>
  <li>Configured DNS settings</li>
  <li>Tested network connectivity</li>
  <li>Joined a Windows client to a domain</li>
  <li>Verified domain login</li>
  <li>Troubleshot basic client-to-server communication</li>
</ul>

<h2>GRC Concepts Demonstrated</h2>

<ul>
  <li>Centralized identity management</li>
  <li>Access control</li>
  <li>Endpoint management</li>
  <li>Device inventory</li>
  <li>Policy enforcement through domain membership</li>
</ul>

<h2>Lessons Learned</h2>

<p>
This lab helped me understand how Windows client machines connect to an Active Directory domain. 
I learned that DNS is important for domain joining because the client needs to find the domain controller. 
I also practiced basic troubleshooting skills by checking IP settings, DNS settings, and network connectivity.
</p>
