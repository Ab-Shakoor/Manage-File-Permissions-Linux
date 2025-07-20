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

The organization determined that the owner type of other should not have write permissions. The following screenshot shows how I used the **(chmod)** command to change the write permissions for the other in the **(project_k.txt)** file. Then, I used the **(ls -la)** command to review the updates I made:

<p align="center">
<img src="https://i.imgur.com/UbvHhi7.png" height="100%" width="80%" alt="Manage File Permissions in Linux"/>

<br />

The organization also determined that the **(project_m.txt)** file is a restricted file and should not be readable or writable by the group or other. The following screenshot shows how I used the **(chmod)** command to change the read permissions for the group in the **(project_m.txt)** file. Then, I used the **(ls -la)** command to review the updates I made:

<p align="center">
<img src="https://i.imgur.com/KEXHYFj.png" height="100%" width="80%" alt="Manage File Permissions in Linux"/>

<br />

<h2>Change file permissions on a hidden file</h2>

The file **(.project_x.txt)** is a hidden file that has been archived and should not be written to by anyone, but the user and group should still be able to read this file. The following screenshot shows how I used the **(chmod)** command to remove writing priviliges for the user and group from the **(.project_x.txt)** file, while also allowing reading priviliges for the group. This ensures both the user and the group can read, but not write to, the file. I then reviewed the updates I made using the **(ls -la)** command.

<p align="center">
<img src="https://i.imgur.com/6793lwm.png" height="100%" width="80%" alt="Manage File Permissions in Linux"/>

<br />


<h2>Change directory permissions</h2>

The organization determined that only the **(researcher2)** user should be allowed to access the **(drafts)** directory and its contents, which means only **(researcher2)** should have execute privileges. The following screenshot shows how I used the **(chmod)** command to remove execute priviliges for the group from the **(drafts)** directory. Then, I used the **(ls -la)** command to review the updates I made. 

<p align="center">
<img src="https://i.imgur.com/MQTsfaU.png" height="100%" width="80%" alt="Manage File Permissions in Linux"/>
<b> </b>


<h2>Summary</h2>
I changed multiple permissions to match the level of authorization my organization wanted for files and directories in the (projects) directory. I checked permissions for the directory using (ls -la), then I used the (chmod) command multiple times to accurately change permissions according to the needs of my organization, and after each time, I reviewed the changes done using (ls -la) to confirm the changes made. 


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
