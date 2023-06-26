# Recap Session

## su

The su command is used to switch to root user without changing the user.

## finger

Finger command is a user information lookup command which gives details of all the users logged in. This tool is generally used by system administrators. It provides details like login name, user name, idle time, login time, and in some cases their email address even. This tool is similar to the Pinky tool but the Pinky tool is just the lightweight version of this tool.

## Password file

/etc/shadow contains all the passwords of the users [Passwords are hashed]

## Environment Variables

In Terminal Scripting we use Environment Variables just like other languages.

Creating a variable [This environment variable will only be available for the given instance]:
FName="suhaan"
echo "$FName"

Displaying the path variable:
echo $PATH

## Finding the path of the software

We can use the which command to find the path of the java:
which java

## export

We use export to add a variable to the environment, eg. export USER_NAME="suhaan"

To print all the environment variables we can use, printenv command

## Vi Editor

Different modes of vi Editor:

1. Command Mode
2. Insert Mode
3. Visual Mode

## kill Command

The total number of Signals available are 62.
2 Signals are reserved for the system.

## Difference between directory and file

In Linux or open source, every thing is a file.

File is of type c:

- b block (buffered) special
- c character (un-buffered) special
- d directory
- p named pipe (FIFO)
- f regular file
  l symbolic link; this is never true if the -L option or the -follow option is in effect, unless the
  symbolic link is broken. If you want to search for symbolic links when -L is in effect, use -xtype.
- s socket
- D door (Solaris)

## grep

We can use grep command to find text in a file.

## ls -l 1st Column

The 3 Basic Permissions:

1. Read

   - Directory: If we have read access to the directory then we can see the files listed in it but not the content.
   - File: If we have read access to the directory then we can read the content of the file.

2. Write

3. Execute(x)

In the 10 Char at first column:
First char is for the type of file.
3 are for read, write and execute for user.
next 3 for group.
next 3 for others.

### Removing the write permission for a file

- chmod -w name.txt

## Links

We can create file links using the ln command

There are two types of links :

1. Soft Link or Symbolic links
2. Hard Links

These links behave differently when the source of the link (what is being linked to) is moved or removed. Symbolic links are not updated (they merely contain a string which is the path name of its target); hard links always refer to the source, even if moved or removed.

- Hard Link: $ ln [original filename] [link name]
- Soft Link: $ ln -s [original filename] [link name]
