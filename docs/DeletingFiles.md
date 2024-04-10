# Deleting Files


!!! info
    These instructions are intended for windows users.

    These commands do may not work on external cloud drives (i.e., Google Drive, oneDrive, etc.).

    User is expected to have a file to delete for this section.

<b>Introduction</b> 

Welcome to the definitive guide on deleting files using the Windows Command Prompt. 
This section is designed to provide you with the necessary command-line skills to 
remove files and directories efficiently. While file deletion is a fundamental 
operation, it's essential to approach it with caution. This guide will not only 
show you how to execute deletions but also how to ensure that you're deleting only 
what you intend to remove, preventing accidental loss of valuable data.

<b> 1. Open the Command Line </b> 

Open the Command Prompt by pressing `Windows Key + R`, typing `cmd`, and pressing 
Enter. 

<b> 2. List Files </b>

List the files in a directory before deletion: 
```bash
dir /b
```

<p> <b> 3. Delete a Single File</b> </p>
!!! warning
    The following steps deletes your file! Don't use the command if you 
    don't want to delete the file!

<ol> Delete a single file using the `del` command: </ol>
```bash
del [filename].txt
```

<i>For example:</i>
```bash
del file.txt
```

<b> 4.Confirm Deletion</b>
<ol> Verify that the file has been deleted:</ol>

```bash
dir /b
```

<b> 5. Delete Multiple Files</b>
!!! warning
    The following steps will delete multiple file! Don't use the command 
    if you don't want to delete your files!

<ol> Use wildcards to delete multiple files:</ol>

```bash
del *.txt
```

<b> 6. Delete Files Recursively</b>
!!! warning
    The following steps will delete multiple file! Don't use the command 
    if you don't want to delete your files!
<ol> Delete files recursively from subdirectories with the `/s` flag:</ol>

```bash
del /s *.txt
```

<b> 7. Delete Directories</b>
!!! warning
    The following steps will delete directories! Don't use the command if 
    you don't want to delete your directories!
<ol> Remove entire directories using `rmdir` or `rd`: </ol>

```bash
rmdir /s /q C:\path\to\directory
```

<b> 8. Secure Deletion</b>
<ol> For secure deletion, use a third-party tool like `sdelete` from Sysinternals: </ol>

```bash
sdelete -p 3 filename.txt
```

<b> 9. Empty Recycle Bin</b>
!!! warning
    The following steps will empty your recycle bin! Don't use the command 
    if you don't want to empty your recycle bin!
<ol> Empty the recycle bin via the command line: </ol>

```bash
rd /s /q C:\$Recycle.Bin
```


<b>Conclusion</b>

You have now mastered the various methods of deleting files and directories using 
the Command Prompt. While the power to remove data with such efficiency is 
invaluable, always remember the importance of double-checking your commands to 
avoid unintended data loss. These command-line skills will serve you well in 
maintaining a clean and organized digital space, but they come with the 
responsibility to use them wisely and judiciously. As you continue to use these 
commands, you'll develop a keen sense of precision and caution, enhancing your 
overall computing practices.