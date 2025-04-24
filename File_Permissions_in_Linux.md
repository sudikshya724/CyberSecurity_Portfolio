In this project, I took on the role of a security specialist, ensuring proper configuration of file and directory permissions for a research team. 
Using various Linux commands, I verified existing permission settings, interpreted what they meant, and made adjustments to access controls where necessary. 
This approach helps maintain a secure environment by limiting unauthorized access.

Checking File and Directory Details
To check the details of files and directories, use:

ls -la /home/researcher2/projects
Understanding the Permissions String
Each file or directory listed will show a 10-character permissions string. Here's how to interpret it:

1st character: File type

- = regular file

d = directory

l = symbolic link

2nd–4th characters: Owner’s permissions

r = read

w = write

x = execute

5th–7th characters: Group’s permissions

8th–10th characters: Others’ permissions

Example:
-rw-r--r--
This means it's a regular file where the owner can read/write, while the group and others can only read it.

Changing File and Directory Permissions
1. Remove write permission from others on a file:


chmod o-w /home/researcher2/projects/project_m.txt
2. Remove write permission from others on a hidden file:
(Note: There was a typo in the original command — missing space and misnamed file.)


chmod o-w /home/researcher2/projects/.project_x.txt
3. Change directory permissions to 700 (owner: all access, others: no access):
(Note: There was a typo — chrod should be chmod.)


chmod 700 /home/researcher2/projects/drafts

Summary
During this project, I reviewed and managed the permissions on several files and folders used by a research team. 
I used the ls -la command to view current permissions and analyzed the 10-character strings to understand access levels.
I then used the chmod command to make necessary updates: removing write permissions for unauthorized users, securing hidden files, 
and limiting access to certain directories. These actions are essential for safeguarding sensitive research materials from potential security threats.
