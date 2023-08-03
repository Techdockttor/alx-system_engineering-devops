# 0x01-shell_permissions

This directory contains several shell scripts related to managing file permissions in Linux. Below is a brief description of each script:

## 1. change_permissions.sh

Description: This script changes the permissions of a file or directory according to the specified mode.

Usage:
#!/bin/bash
chmod <permission_mode> <file_or_directory>

## 2. set_ownership.sh

Description: This script sets the ownership of a file or directory to the specified user and group.

Usage:
#!/bin/bash
chown <user>:<group> <file_or_directory>

## 3. grant_execute_permission.sh

Description: This script grants execute permission to a specified user on a given file.

Usage:
#!/bin/bash
chmod u+x <file>

## 4. revoke_read_permission.sh

Description: This script revokes read permission from a specified user on a given file.

Usage:
#!/bin/bash
chmod u-r <file>

## 5. allow_group_write.sh

Description: This script allows group write permission on a specified directory.

Usage:
#!/bin/bash
chmod g+w <directory>

## 6. remove_other_permissions.sh

Description: This script removes all permissions for others on a specified file or directory.

Usage:
#!/bin/bash
chmod o= <file_or_directory>

## 7. change_permission_recursive.sh

Description: This script recursively changes the permissions of all files and directories within a given directory to the specified mode.

Usage:
#!/bin/bash
chmod -R <permission_mode> <directory>
EOF

# Make all scripts unexecutable
chmod -x change_permissions.sh set_ownership.sh grant_execute_permission.sh revoke_read_permission.sh allow_group_write.sh remove_other_permissions.sh change_permission_recursive.sh
