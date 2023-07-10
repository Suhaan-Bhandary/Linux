# SORT GREP SED and AWK

## Linux Pipes

### What is a Pipe in Linux?

- The symbol '|' denotes a pipe.
- Use Pipes to run two commands consecutively.
- Helps in creating powerful command.

## grep

- Searching a text in file
- Scan a document

```bash
    cat trial.txt | grep 5 -n -1
```

- -v can be used to search for words which are not.
- -c displays only the count of matching lines.
- -n shows the matching line and its number.
- -i match both case.
- -l shows just the name of the file with the string.
- -w for whole word

## sort

- It can be used to sort the output
