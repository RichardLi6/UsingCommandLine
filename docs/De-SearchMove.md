# Search and Move Files

!!! info
These instructions are intended for windows users
These commands do may not work on external cloud drives (i.e., Google Drive, oneDrive, etc.).


## Introduction
Welcome to the world of command-line mastery. As you embark on this journey, you
will learn to wield the powerful tools offered by the Windows Command Prompt. The
command line offers precision and speed, qualities essential for effective file
management. From finding text files tucked away in nested directories to moving
batches of data to new homes, the skills you acquire today will transform your
tasks into a symphony of keystrokes.

## <b> Open the Command Line</b> 
Open the Command Prompt by pressing `Windows Key + R`, typing `cmd`, and pressing
Enter.

## <b> Search for Files</b> 
Use the `dir` command to search for files. For example, to find all `.txt` files in
a directory:

<i>For example</i>, to find all `.txt` files in a directory:
```bash
dir /s /b *.txt
```
<i>For example</i>, to find a specific .txt file in a directory:
```bash
dir /s /b [filename].txt
```
<i>For example</i>, to find a file named 'file.txt' in a directory:
```bash
dir /s /b file.txt
```

## <b> Move the File</b> 
Move a file to a new location with the `move` command:

```bash
move C:\[path]\[to]\[source]\[file name].txt C:\[path]\[to]\[destination]\
```
<i>For example</i> To move 'file.txt' from downloads of user Richard to documents:
```
move C:\Users\Richard\Downloads\file.txt C:\Users\Richard\Documents
```

## <b> Verify the Move</b> 
Check that the file has been moved to the new location:

```bash
dir C:\path\to\destination\
```

## <b> Copy the File</b> 
Copy a file with the `copy` command:

```bash
copy C:\path\to\source\filename.txt C:\path\to\destination\filename.txt
```

## <b> Rename the File</b> 
Rename a file using the `ren` or `rename` command:

```bash
ren C:\path\to\filename.txt newfilename.txt
```

## <b> Search Within Files</b> 
Search for a specific string within files using `findstr`:

```bash
findstr /s "searchstring" *.txt
```

## <b> Organize Search Results</b> 
Sort the search results by name or date using `dir` with sorting flags:

```bash
dir /b /o:n *.txt
```

## <b> Selective Move</b> 
Move only certain files using wildcards with `move`:

```bash
move C:\path\to\source\*.txt C:\path\to\destination\
```

## <b> Create Directory Structure</b> 
Recreate the directory structure in the destination using `xcopy`:

```bash
xcopy /t /e C:\path\to\source\ C:\path\to\destination\
```
## Conclusion
Congratulations on completing this guide to searching and moving files with the 
Windows Command Prompt. These steps are just the beginning of what's possible with
command-line tools at your fingertips. As you grow more comfortable with these 
commands, you'll find that they become second nature, making you a more adept and
efficient user. The command line is a gateway to a vast world of advanced computing
operations—continue exploring, and you'll uncover even more powerful ways to manage
your digital environment.






