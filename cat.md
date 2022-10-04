---
title: cat Linux Command
description: cat command is used to create, read & concatenate files in Linux/ Unix machines
created: 2019-08-21
updated: 2019-08-21
---

`cat` command is used to create, read & concatenate files in Linux/ Unix machines. 

## 1. Creating a file with content
Lets create a file with name `file1.txt` and put following three lines of content into it. 

First you need to run the following command to create a file

```sh
cat >file1.txt
```
When you press enter after the above command, it waits for the file content input. You can give multi line input and once you are done you need to press `CTRL + D` to save and exit. 


## 2. Displaying file contents 
Following command shows the content of given file
```sh
cat file1.txt
```
## 3. Display content from multiple files
Following command shows content from file1.txt followed by content from file2.txt

```sh
cat file1.txt file2.txt
```

## 4. Display Line Numbers before every line 

Following command prefixes line numbers before each line from content

```sh
cat -n file1.txt
```
Following is an example for that 

```sh
$ cat -n file1.txt
     1	line-1
     2	line-2
     3	line-3
     4	line-4
```


## More Options

|Option| Description|
|---|---|
|`-e`|Shows `$` at the end of the content|
|`-t`|To see tabs in file, this shows tabs with `^I`|
|`-s`|removes repeated empty lines in content|
|`cat test > test1`|redirect the standard output of a file into a new file|
