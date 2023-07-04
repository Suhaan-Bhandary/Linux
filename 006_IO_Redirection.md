# I/O Redirection

## Output Redirection

The '>' is used for output redirection.

The below command will write the output of ls to listing.txt

```bash
    ls -la > listing.txt
```

Note:
If pre-existing file name is used then the content will be overwritten.

The '>>' is used for appending output to the file.

```bash
    echo hi >> listing.txt
```

## Input Redirection

The '<' is used for input redirection.

## File Descriptors

In linux everything is a file.
Even a device is considered to be a file.

Every file has a FD[File Descriptor]

### FD

- Standard Input FD0 [STDIN]
- Standard Output FD1 [STDOUT]
- Standard Error FD2 [STDERR]

## Error Redirection

```bash
telnet localhost 2> error.txt
```

Notice that 2 is used to define the FD of the file.

## Complex Example

```bash
    ls trial.txt a > dirlist 2>&1
```

<!-- >& is used to redirect the output of FD 2 to FD 1 -->
