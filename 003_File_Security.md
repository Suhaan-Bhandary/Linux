# File Permission

Since linux is a multi-user operating system, it requires file level security.

## Authorization Levels

1. Ownership
2. Permission

## Ownership

Types of owner:

- user or creator
- group
- other[permission to all]

[d user group other] is the output of ls -al
r = read
w = write
x = execute
\- = not set

By default user is added to the same group as their name, so suhaan is added to group suhaan.

## chmod

chmod stands for `change mode`, it is used to set permissions on a file/directory for owner, group or world.

### Two types to use the chmod command

- Absolute Mode

  - 0 : ---
  - 1 : --x
  - 2 : -w-
  - 3 : -wx
  - 4 : r--
  - 5 : r-x
  - 6 : rw-
  - 7 : rwx

- Symbolic Mode
  - In this mode we can modify only one user.
  - Operator:
    - [+] Adds a permission to a file or directory
    - [-] Remove a permission to a file or directory
    - [=] Sets the permission and overrides the permissions set earlier [It sets rwx if provided else -]
  - User
    - u is User
    - g is group
    - o is other
    - a is all

## chown

chown is used to change ownership and group of a file.

- chown user <filename>
- chown user:group <filename>
- chgrp group <filename> [this is used to change only the group]

## newgrp

This is used to change the group of the user

- newgrp groupName

User group is changed to groupName.
Two groups cannot have same group.

## groupadd

This command will create a new group with the given name.
Command: `groupadd groupName`

## groupdel

This command is used to remove a delete a group.

## ln

This command is used to create a file link, the link is hard by default and -s can be used to make it soft.
