# Topic 4: Understanding and Applying Linux Permissions

## Understanding File Permissions

This lab introduced me to how Linux controls access to files and directories. I learned that permissions determine whether a user can read, write or execute a file. This is important because not every user should have unrestricted access to system resources.

One of the commands I explored was:

`ls -l`

This displays file and directory permissions, along with ownership information. I also learned about `chmod`, which changes permissions, and `chown`, which changes file ownership.

## Understanding Permission Values

I learned how Linux represents permissions using numbers:

- 7 represents read, write and execute (rwx).
- 6 represents read and write (rw-).
- 5 represents read and execute (r-x).
- 4 represents read only (r--).
- 0 represents no permissions (---).

Understanding these values helped me see how permissions can be assigned to the file owner, group and other users.

## Reflection

This activity helped me understand why Linux permissions are important for protecting files and controlling access. In a server environment, incorrect permissions could allow unauthorised users to modify or access important files. These concepts are useful for system administrators and cybersecurity professionals who need to maintain the security of Linux systems.
