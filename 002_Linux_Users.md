# Users In Linux

Linux is a multi user system, so their is a requirement for Linux Admin to take care of the users and groups.

## whoami

It tells you about the system's username

## who

The who command gives the information about the users logged on to the system.

## w

This command tells about the users who are logged in and what are they doing.

## su

The su command can be used to run as other user without closing the shell.

```bash
su OtherUserName
```

<!-- Note: By default, some Linux systems like Ubuntu, don't have a password set for root user. It means you can't login as root user. -->

## changing password of a user

The command `passwd` can be used to change the password of the current user.
The command `passwd userName` can be used to change the password of a particular user.

## Creating multiple users

There are two types of users:

1. Standard
2. Administrator

- The below command will create a new user

```bash
sudo adduser harshini
```

- We can also use gui for creating the user from the settings

## Removing the user

- First we have to remove the password info of the user

```bash
sudo passwd -l otherUserName
```

- Now we remove the account

```bash
sudo userdel -r otherUserName
```

## Adding User to a group

groupmod with tab shows all the available groups on the system.

```bash
sudo usermod -a -G groupName userName
```

To view if the user is added in the group

```bash
cat /etc/group | grep userName
```

## Removing User from a group

```bash
sudo deluser userName groupName
```

## Using UI for managing users and groups

```bash
sudo apt-get install gnome-system-tools
```

## Finger Command

It is used to Procure information of the users on a linux machine.
eg: finger or finger userName

## Shadow File

Shadow files are the encrypted user passwords which are kept in /etc/shadow. This file is read-only directory and can be read only by root.
