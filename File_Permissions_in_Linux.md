In this project, I took on the role of a security specialist, ensuring proper configuration of file and directory permissions for a research team. 
Using various Linux commands, I verified existing permission settings, interpreted what they meant, and made adjustments to access controls where necessary. 
This approach helps maintain a secure environment by limiting unauthorized access.

Check file and directory details
ls -la /home/researcher2/projects

Explain the permissions string
-rw-rw-rw-

Modify file permissions
chmod o-w /home/researcher2/projects/project_k.txt

Modify permissions on a hidden file
chmod 440 /home/researcher2/projects/.project_x.txt

Modify directory permissions
chmod 700 /home/researcher2/projects/drafts

Summary
During this project, I reviewed and managed the permissions on several files and folders used by a research team. 
I used the ls -la command to view current permissions and analyzed the 10-character strings to understand access levels.
I then used the chmod command to make necessary updates: removing write permissions for unauthorized users, securing hidden files, 
and limiting access to certain directories. These actions are essential for safeguarding sensitive research materials from potential security threats.
