# Deleting Files


!!! info
    These instructions are intended for windows users.

    These commands do may not work on external cloud drives (i.e., Google Drive, oneDrive, etc.).

    User is expected to have files and directories to delete for this section.

<b>Introduction</b> 

The following is the guide on deleting files using the Windows Command Prompt. This section is meticulously designed to provide you with the necessary command-line skills to remove files and directories efficiently. While file deletion is a fundamental operation, it's essential to approach it with caution. This guide will not only show you how to execute deletions but also how to ensure that you're deleting only what you intend to remove, preventing accidental loss of valuable data.

<b> 1. Open the Command Line </b> 

Open the Command Prompt by pressing `Windows Key + R`, typing `cmd`, and pressing 
Enter. 

<figure markdown="span">
![Command Prompt](./CommandLine.png){ height="800"}
<figcaption>Command Prompt window</figcaption>
</figure>

<b> 2. Find the file </b> 

If you know the directory of the file already, you can move to step 4.

Navigate to your desired directory using the `cd` command for file deletion. If you already know the file name for deleting, try these commands to find location.
```bash
C:\[Users]\[user]>dir /s /b [file name]
```
For example:
```
C:\Users\Richard>dir /s /b text.txt
```
!!! tip
    If you only know the first few letters of the file name, do the command below
    ```bash
    C:\[Users]\[user]>dir /s /b *[file name]*
    ```

    For example,
    ```
    C:\Users\Richard>dir /s /b *tex*
    ```
<b> 3. Copy the file location </b> 

Copy the file location of the address by highlighting the directory using ctrl + c.

For example if I'm looking for the txt file, only copy the address before the file.
```
C:\Users\Richard\Downloads\text.txt
```
I would only copy the bottom portion.
```
C:\Users\Richard\Downloads\
```


<b> 4. Navigate to file location </b>

Navigate to your desired directory using the `cd` command where you want to delete files.

```
cd [directory address]
```

<i> For Example: </i>
```bash
cd C:\[Users]\[user]\Documents
```


<b> 5. List Files </b>
List the files in a directory before deletion: 
```bash
dir /b
```

<b> 6. Delete a Single File</b> 
!!! warning
    The following steps deletes your file! Don't use the command if you 
    don't want to delete the file!

Delete a single file using the `del` command: 
```bash
del [filename].txt
```

<i>For example:</i>
```bash
del file.txt
```

<b> 7. Confirm Deletion</b>

Verify that the file has been deleted:

```bash
dir /b
```

<b> 8. Delete Multiple Files</b>
!!! warning
    The following steps will delete multiple file! Don't use the command 
    if you don't want to delete your files!

Use wildcards to delete multiple files:

```bash
del *.txt
```

<b> 9. Delete Directories</b>

!!! warning
    The following steps will delete directories! Don't use the command if 
    you don't want to delete your directories!
Remove entire directories using `rmdir` or `rd`: 

```bash
rmdir /s /q C:\path\to\directory
```

<b> 10. Secure Deletion</b>

For secure deletion, use a third-party tool like `sdelete` from Sysinternals: 

```bash
sdelete -p 3 filename.txt
```

<b> 11. Empty Recycle Bin</b>
!!! warning
    The following steps will empty your recycle bin! Don't use the command 
    if you don't want to empty your recycle bin!

Empty the recycle bin via the command line: 

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