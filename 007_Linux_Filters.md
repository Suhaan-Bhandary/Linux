# Linux Filters

## Displaying the data

- The below command displays the whole file, we can use -n to display the number of lines

```bash
cat filename
```

- To display only first 10 lines we can use head, we can also provide -n 5 for getting 5 lines

```bash
head filename
```

- To display only last 10 lines we can use head, we can also provide -n 5 for getting 5 lines

```bash
tail filename
```

- Getting the middle lines from a files, we have to use both the files
- eg, we have to get 5 to 8 line

```bash
head trial.txt -n 8 | tail -n 4
```

### Note

    - 8 is the last line number
    - 4 is (high - low + 1)

## More

- more command is used to only display single page, and we can press space to get the next page.
- q can be use to exit
- enter can be used to see line by line

## less

- less can navigate to pre and next page both.
- more cannot go to previous page.
- p is used to go to previous page.

## tee

- It is used to save the output to the file.

## tr

- tr is used to replace the text with the new one.

## sort

- sort is used to sort the file contents and display them.

## gzip

- Gzip (GNU zip) is a compressing tool, which is used to truncate the file size. By default original file will be replaced by the compressed file ending with extension (.gz).

- gzip, and gunzip
