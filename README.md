<h1>Manage File Permissions in Linux</h1>


<h2>Project Description</h2>
In this project, I examine existing permissions on the file system and determine if the permissions match the authorization that should be given. If they do not match, I modify the permissions to authorize the appropriate users and remove any unauthorized access</a>.
<br />

<h2>Check file and directory details</h2>
<p align="center">
<img src="https://i.imgur.com/NNPdg2d.png" height="100%" width="80%" alt="Manage File Permissions in Linux"/>
 
- The first line of the screenshot displays usage of the **(cd)** command to navigate to the **(projects)** directory.
- The second line of the screenshot displays usage of the **(ls -l)** command to list the contents and permissions of the **(projects)** directory.

<br />

To check hidden files, the following screenshot displays usage of the **(ls -la)** command, revealing the hidden file **(.project_x.txt)**: 
<p align="center">
<img src="https://i.imgur.com/r2KkhZk.png" height="100%" width="80%" alt="Manage File Permissions in Linux"/>
<br />


<h2>Describe the permissions string</h2>
a 10-character string begins each entry and indicates how the permissions on the file are set. For instance, a directory with full permissions for all owner types would be drwxrwxrwx:

- The 1st character indicates the file type. The d indicates it’s a directory. When this character is a hyphen **(-)**, it's a regular file.
- The 2nd-4th characters indicate the read **(r)**, write **(w)**, and execute **(x)** permissions for the user. When one of these characters is a hyphen **(-)** instead, it indicates that this permission is not granted to the user.
- The 5th-7th characters indicate the read **(r)**, write **(w)**, and execute **(x)** permissions for the group. When one of these characters is a hyphen **(-)** instead, it indicates that this permission is not granted for the group.
- The 8th-10th characters indicate the read **(r)**, write **(w)**, and execute **(x)** permissions for the owner type of other. This owner type consists of all other users on the system apart from the user and the group. When one of these characters is a hyphen **(-)** instead, that indicates that this permission is not granted for other.

The second block of text in the expanded directory listing is the user who owns the file. The third block of text is the group owner of the file.


<h2>Change file permissions</h2>
<p align="center">
<img src="https://i.imgur.com/UbvHhi7.png" height="100%" width="80%" alt="Manage File Permissions in Linux"/>
<b> </b>
<p align="center">
<img src="https://i.imgur.com/KEXHYFj.png" height="100%" width="80%" alt="Manage File Permissions in Linux"/>

<h2>Change file permissions on a hidden file</h2>
<p align="center">
<img src="https://i.imgur.com/6793lwm.png" height="100%" width="80%" alt="Manage File Permissions in Linux"/>
<b> </b>


<h2>Change directory permissions</h2>
<p align="center">
<img src="https://i.imgur.com/MQTsfaU.png" height="100%" width="80%" alt="Manage File Permissions in Linux"/>
<b> </b>


<h2>Summary</h2>

<b> </b>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
