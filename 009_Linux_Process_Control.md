# Linux Process Control

## What is a Process?

- An instance of a program is called a Process.
- Any command that you give to your linux machine starts a new process.

## Types of Processes

- Foreground Processes
- Background Processes

### How to send process to background!!

Which using nautilus in foreground we cannot use the terminal.
So we have to put the process in the background.

Steps:

- start the program
- press ctrl + z
- type `bg` to send process to background
- to bring it back use `fg`

## top

top can be used to show all the process.

## ps

It also shows the processes.
`ps PID`

## kill

killing a process
`kill PID`

## Nice

Default value of all the processes is 0.
nice -n 'Nice Value' process

Lower the nice, higher the priority.

```bash
sudo renice -Value -p PID
```

Priority value — The priority value is the process’s actual priority which is used by the Linux kernel to schedule a task.
In Linux system priorities are 0 to 139 in which 0 to 99 for real-time and 100 to 139 for users.

Nice value — Nice values are user-space values that we can use to control the priority of a process. The nice value range is -20 to +19 where -20 is highest, 0 default and +19 is lowest.

Priority_value = Nice_value + 20

## df

df can be used to see the disk space.

## free

It is used to show the ram.
`free -m` shows in megabyte.
