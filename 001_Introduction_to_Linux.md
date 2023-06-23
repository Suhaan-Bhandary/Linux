# Introduction to Linux

## ls command

1. ls

   - It is used to show directories and files.
   - notice that the color of files and directories is different.
   - ls command only shows files inside the current folder

2. ls -R

   - This command can be used to show all files and folders inside the current folder and sub folders.
   - Here -R means recursive.

3. ls -al

   - This command will show lot of information about the folders and files inside the current directory.
   - 1st column: Shows the file types and Access Permissions
   - 2nd column: Shows the memory blocks
   - 3rd column: Owner of the file
   - 4th column: User Group
   - 5th column: File Size in Bytes
   - 6th column: Last change time

4. ls -a
   - This command can be used to show the hidden files

## cat command

1. cat > trial.txt

   - This command will create a new file, and it will also take the user input for the content of the file, ctrl d to exit after the content is given.

2. cat trial.txt

   - This will show the content of the file.

3. cat trial2.txt >> trial.txt

   - This will append the first file to the next file.
   - Notice that the >> is used to append contents to the file.

4. cat trial1.txt trial2.txt > newFile.txt

   - This command is used to combine file and create a new file with it

## Deleting, Moving and Renaming Files

1. rm test.txt

   - This will remove the test.txt file.

2. mv oldFolderLocation/file.txt newFolderLocation

   - This will move from old location to the new location.
   - If permission denied message is their then we have to use _sudo_ command.
   - sudo command maintains log of the commands so that we can track the usage of it.
   - sudo command is maintained in the terminal for 15 mins.

3. mv oldName newName

   - This command will rename the file.

4. mkdir subfolder

   - This will create a subfolder

5. mkdir dir1 dir2 dir3

   - This command will create multiple directories in one command.

6. rmdir dir1

   - This will delete the directory.
   - Remember that this command can only be used if the dir1 is empty.

## man

This _man_ command is used to display the manual of a command.

## history

This command can be used to display all the commands used on the terminal by the user.

## clear

This command is used to clear the terminal.

## pwd

pwd command is used to show the path of the current directory.

## cd command

- `cd folderPath` This can be used to change the folder to the given path.
- `cd -` this command can be used to go to the previous directory.
- `cd ..` to go to the previous directory.

## Tips

- use tab to get command completions
