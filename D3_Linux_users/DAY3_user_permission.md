Day3 markdown
# Linux User/Group Permissions

1. Introduction
In Linux systems, access to files and directories is controlled through users, groups, and permissions.

2. User Types
*Root User* – Superuser with full system access.
*Regular User* – Limited access for daily tasks.
*System User* – Used by services and background processes.

3. Groups
- A *group* is a collection of users.
- Groups simplify permission management.
- A user can belong to multiple groups.

4. File Permission Types
Each file/directory has three permission types:

`r` – Read (view file / list directory)
`w` – Write (modify file / add-delete files in directory)
`x` – Execute (run file / access directory)

5. Permission Levels
Permissions are assigned to:

`u` – User (Owner)
`g` – Group
`o` – Others

Example:

-rwxr-xr--

Breakdown:
User → `rwx`
Group → `r-x`
Others → `r--`


6. Important Commands

`ls -l` → View file permissions
`chmod` → Change permissions
`chown` → Change file owner
`chgrp` → Change group ownership
`id` → Show user and group IDs
- `groups` → Show user groups

7. Numeric (Octal) Permissions

| Permission | Value |
|------------|-------|
| r          | 4     |
| w          | 2     |
| x          | 1     |

Example:
`chmod 755 file.txt`
7 (rwx) → User
5 (r-x) → Group
5 (r-x) → Others


# Summary
Linux permissions ensure system security by controlling who can read, write, or execute files and directories.
