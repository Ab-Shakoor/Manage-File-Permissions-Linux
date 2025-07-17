<h1>Manage File Permissions in Linux</h1>


<h2>Overview</h2>
In this project, I examine existing permissions on the file system and determine if the permissions match the authorization that should be given. If they do not match, I modify the permissions to authorize the appropriate users and remove any unauthorized access</a>.
<br />

<h2>Objective</h2>
Gain hands-on experience and familiratiy with common every day Active Directory help desk tasks.

<h2>Tools Used</h2>

- <b>VirtualBox</b> 
- <b>Windows Server 2019</b>
- <b>Active Directory</b>

<h2>Key Features</h2>

- <b>Locate users and computers in AD</b> 
- <b>Reset user passwords</b>
- <b>Edit user attributes (title, department, phone)</b>
- <b>Move users between OUs</b>
- <b>Enable Advanced Features and view extra attributes</b>
- <b>View computer properties and trust status</b>
- <b>Create a service account with limited permissions</b>
- <b>Simulate onboarding (create new user and assign to group)</b>
- <b>Simulate offboarding (disable user and move to "Disabled Users" OU)</b>


<h2>Project walk-through:</h2>
<br/>

<p align="center">
<b>Used the "Find" tool in ADUC to locate a specific user by the name "abdullah":
<br/>
 
<br/>
<img src="https://i.imgur.com/x5q6qzL.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />
 
<br/>

---

<p align="center"> 
<br />
Located user `ashakoor` in ADUC, right-clicked and selected “Reset Password”, and applied a temporary password and enforced a reset on next login: 
<br/>

<br/>
<img src="https://i.imgur.com/6roz9ko.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>
<img src="https://imgur.com/W6ZkMXD.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Opened the properties for user `ashakoor` and updated job title and department: 
<br/>

<br/>
<img src="https://i.imgur.com/oyft0Gn.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>

---

<p align="center">
<br />
Moved user `ashakoor` from `_USERS` to `IT_DEPARTMENT` OU:  
<br/>

<br/>
<img src="https://i.imgur.com/QNDoURU.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>
<img src="https://i.imgur.com/8c8FX10.png" height="400%" width="80%" alt="Active Directory Home Lab Steps"/>
<br />

<br/>




<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
