<h1>Active Directory Lab</h1>

<h2>Description</h2>

<p>
This project documents my learning from an Active Directory lab. 
The lab demonstrates how Windows domains are used to centrally manage users, computers, groups, permissions, and security policies in a business environment.
</p>

<p>
Through this lab, I learned about domain controllers, Active Directory users and computers, organizational units, security groups, delegation, Group Policy, authentication, and domain structures such as trees, forests, and trusts.
</p>

<h2>Technologies and Concepts Used</h2>

<ul>
  <li><b>Active Directory Domain Services (AD DS)</b></li>
  <li><b>virtual machine</b></li>
  <li><b>Windows Domain</b></li>
  <li><b>Domain Controllers</b></li>
  <li><b>Organizational Units (OUs)</b></li>
  <li><b>Security Groups</b></li>
  <li><b>Group Policy</b></li>
  <li><b>Authentication</b></li>
  <li><b>Trees, Forests, and Trusts</b></li>
</ul>

<h2>Skills Practiced</h2>

<ul>
  <li>Active Directory administration</li>
  <li>Learning how users and computers are managed in a domain</li>
  <li>Understanding organizational units and security groups</li>
  <li>Learning how delegation supports support tasks</li>
  <li>Understanding how Group Policy applies rules to users and computers</li>
  <li>Connecting Active Directory concepts to access control</li>
</ul>

<h2>Lab Walk-Through</h2>

<h3 align="center">Step 1: Review Active Directory Users and Computers</h3>

<p align="center">
  <img src="https://i.imgur.com/keyDRiK.png" width="80%" alt="Active Directory Users and Computers"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I opened Active Directory Users and Computers to review the domain structure. 
This showed the main containers and organizational units, including users, computers, domain controllers, and department-based OUs.
</p>

<br />

<h3 align="center">Step 2: Review Organizational Units</h3>

<p align="center">
  <img src="https://i.imgur.com/Rr7n3xr.png" width="80%" alt="Creating an Organizational Unit in Active Directory"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I reviewed Organizational Units in Active Directory and created a new OU named <code>Students</code>. 
This helped me understand how OUs are used to organize users and computers into groups such as departments, teams, or device categories.
</p>

<br />

<h3 align="center">Step 3: Manage Users in an Organizational Unit</h3>

<p align="center">
  <img src="https://i.imgur.com/MTUwg73.png" width="80%" alt="Managing users in an Organizational Unit"/>
  <img src="https://i.imgur.com/1xejpql.png" width="80%" alt="Managing users in an Organizational Unit"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I opened an Organizational Unit in Active Directory Users and Computers and reviewed the user accounts inside it. 
I also practiced disabling a user account, which is a common account management task in Active Directory.
</p>

<br />

<h3 align="center">Step 4: Enable Advanced Features to Delete an OU</h3>

<p align="center">
  <img src="https://i.imgur.com/2Y2ZWtV.png" width="80%" alt="Enable Advanced Features in Active Directory"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I enabled <code>Advanced Features</code> in Active Directory Users and Computers. 
This allowed me to view additional object settings needed to manage protected Organizational Units.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/ANEjlts.png" width="80%" alt="Disable accidental deletion protection"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I opened the Organizational Unit properties and went to the <code>Object</code> tab. 
Then I unchecked <code>Protect object from accidental deletion</code> so the extra OU could be removed.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/h3gStDG.png" width="80%" alt="Delete Organizational Unit confirmation"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
After removing accidental deletion protection, I deleted the extra Organizational Unit from Active Directory.
</p>

<br />

<h3 align="center">Step 5: Delegate Password Reset Permissions</h3>

<p align="center">
  <img src="https://i.imgur.com/ODwnBoG.png" width="80%" alt="Select Delegate Control option"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I right-clicked the <code>Sales</code> Organizational Unit and selected <code>Delegate Control</code>. 
Delegation allows specific users to perform limited administrative tasks without giving them full administrator access.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/a0r7cr9.png" width="80%" alt="Delegation of Control Wizard users and groups"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
The Delegation of Control Wizard opened and asked me to select the users or groups that would receive delegated permissions.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/uFZAeDO.png" width="80%" alt="Enter Phillip for delegation"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I entered the user <code>philip</code> and clicked <code>Check Names</code> to verify the account in Active Directory.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/I6e3Y3H.png" width="80%" alt="Verified Phillip user account"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
Active Directory verified the user account as <code>Phillip (phillip@thm.local)</code>.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/bmtKoZX.png"" width="80%" alt="Phillip added to Delegation Wizard"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I added <code>Phillip</code> to the delegation list and continued to the next step.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/O4usAMy.png"" width="80%" alt="Delegate password reset task"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I selected <code>Reset user passwords and force password change at next logon</code>. 
This gives Phillip limited permission to help users with password issues.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/wOCCj3j.png" width="80%" alt="Complete Delegation of Control Wizard"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I completed the Delegation of Control Wizard. 
This confirmed that Phillip was delegated password reset permissions for the <code>Sales</code> Organizational Unit.
</p>

<br />

<h3 align="center">Step 6: Test Delegated Password Reset Permissions</h3>

<p align="center">
  <img src="https://i.imgur.com/O1q6BuI.png" width="80%" alt="Phillip resetting Sophie password with PowerShell"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I tested the delegated permissions by using <code>Phillip</code>, an IT support user, to reset <code>Sophie</code>'s account password with PowerShell. 
This confirmed that Phillip had limited permission to perform password reset tasks without being a full domain administrator.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/5n9Cxjh.png" width="80%" alt="Successful login after Sophie password reset"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I verified that Sophie’s account password was changed successfully by logging in with the updated account credentials. 
This confirmed that the delegated password reset permissions worked correctly.
</p>

<br />
<h3 align="center">Step 7: Organize Computer Objects into a Workstations OU</h3>

<p align="center">
  <img src="https://i.imgur.com/L7zkEEQ.png" width="80%" alt="Create new Organizational Unit"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I created a new Organizational Unit named <code>Workstations</code> to organize computer objects in Active Directory.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/VHNcl1M.png" width="80%" alt="Create Workstations Organizational Unit"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I confirmed the creation of the <code>Workstations</code> OU. This OU will be used to separate workstation computer accounts from the default Computers container.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/KcGTjyI.png" width="80%" alt="Move computer objects to Workstations OU"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I selected the workstation computer objects and moved them into the new <code>Workstations</code> OU. 
This helps keep computer accounts organized and makes it easier to apply policies to specific device groups.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/KcGTjyI.png" width="80%" alt="Workstations OU with computer objects"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I verified that the workstation computer objects were successfully placed inside the <code>Workstations</code> OU.
</p>

<br />

<h3 align="center">Step 8: Review and Update Group Policy Password Settings</h3>

<p align="center">
  <img src="https://i.imgur.com/PCCey8P.png" width="80%" alt="Edit Default Domain Policy"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I opened Group Policy Management and selected the option to edit the <code>Default Domain Policy</code>.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/KFxM3KY.png" width="80%" alt="Review password policy settings"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
Inside the Group Policy Management Editor, I reviewed the password policy settings under <code>Account Policies</code>.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/6tCRlYy.png" width="80%" alt="Set minimum password length"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I changed the <code>Minimum password length</code> policy to require at least <code>10</code> characters.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/28Vgk3W.png" width="80%" alt="Verify updated minimum password length"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I verified that the minimum password length setting was updated from <code>7 characters</code> to <code>10 characters</code>.
</p>

<br />

<h3 align="center">Step 9: Create and Apply Group Policies</h3>

<p align="center">
  <img src="https://i.imgur.com/uiaYjXj.png" width="80%" alt="Create Restrict Control Panel Access GPO"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I created a new Group Policy Object named <code>Restrict Control Panel Access</code>. 
This policy will be used to limit access to Control Panel and PC settings for selected users.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/UnoCqTx.png" width="80%" alt="Open Control Panel policy setting"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I opened the Group Policy Management Editor and located the setting for <code>Prohibit access to Control Panel and PC settings</code>.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/6bRLk1c.png" width="80%" alt="Enable Control Panel restriction"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I enabled the policy setting to block users from opening Control Panel and PC settings.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/qH75MO0.png" width="80%" alt="Verify Control Panel policy enabled"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I verified that the Control Panel restriction policy was enabled in the Group Policy Management Editor.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/ac0Gi7O.png" width="80%" alt="Link Control Panel GPO to Organizational Units"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I linked the <code>Restrict Control Panel Access</code> policy to selected Organizational Units so the setting would apply to users in those OUs.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/JWbmKNr.png" width="80%" alt="Confirm GPO linked to Management OU"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I confirmed that the Group Policy Object was linked to the <code>Management</code> OU.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/nl7Brr8.png" width="80%" alt="Create Auto Lock Screen GPO"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I created another Group Policy Object named <code>Auto Lock Screen</code> to configure automatic workstation locking.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/rNxLFdN.png" width="80%" alt="Open machine inactivity limit policy"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I located the <code>Interactive logon: Machine inactivity limit</code> policy setting in the Group Policy Management Editor.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/XKSyH9a.png" width="80%" alt="Set machine inactivity limit"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I enabled the machine inactivity limit and set the workstation to lock after <code>300</code> seconds of inactivity.
</p>

<br />

<p align="center">
  <img src="https://i.imgur.com/u0iZGAu.png" width="80%" alt="Control Panel access restricted"/>
</p>

<p style="background-color:#e8f4ff; padding:12px; border-left:4px solid #2f80ed; border-radius:6px;">
I tested the policy on a workstation and confirmed that access to Control Panel and PC settings was blocked by policy.
</p>

<br />

<h2>Skills Demonstrated</h2>

<ul>
  <li>Reviewed Active Directory domain structure</li>
  <li>Created and organized Organizational Units (OUs)</li>
  <li>Managed and disabled user accounts</li>
  <li>Delegated password reset permissions</li>
  <li>Reset a user password using delegated access</li>
  <li>Moved computer objects into a Workstations OU</li>
  <li>Updated password policy settings</li>
  <li>Created and linked Group Policy Objects</li>
  <li>Restricted Control Panel access using Group Policy</li>
  <li>Configured automatic workstation lockout</li>
</ul>
</ul>

<h2>Lessons Learned</h2>

<p>
This lab helped me understand how Active Directory is used to manage users, computers, permissions, and policies in a business environment. 
I learned the purpose of domain controllers, organizational units, security groups, delegation, Group Policy, authentication, trees, forests, and trusts.
</p>

<p>
This project helped me connect technical Active Directory skills to real-world identity management, access control, least privilege, centralized administration, and policy enforcement.
</p>
