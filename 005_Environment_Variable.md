# Environment Variable

Platform = Operating System + Processor

## What is a variable?

- It is a memory location for storing a value.
- Refereed to with its symbolic name.
- The value stored can be display, deleted, edited and re-saved.

## Common Environment variable

- PATH contains a colon separated list of directories in which you system looks for executable files.
- USER is the username.
- HOME is the path to the user's home directory.
- EDITOR is the program which edits the content of the files.
- UID is the user's unique ID.
- TERM is the default terminal emulator.
- SHELL displays the shell being used by the user.
- ENV displays all the environment variables.

## Displaying a variable

```bash
    echo $PATH
```

## Creating a variable

```bash
    VARIABLE=value123
```

Note: Don't leave space in between = and variables.

## Creating a variable using export

Using export we can use variables in subprocess

```bash
    export VARIABLE=value123
```

## Creating a persistent variable

The above 2 methods creates a variable for the current session, but it is removed when we close the shell.

```bash
    vim ~/.bashrc

    # Inside the .bashrc
    export name="suhaan"

    # Update the .bashrc
    source .bashrc
```

## Global variable

Go to /etc/ and add the variable `export global="hi"` in the

## Un-setting a variable

```bash
    unset VARIABLE
```
