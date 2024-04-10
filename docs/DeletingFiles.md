# Deleting Files


!!! info
    These instructions are intended for windows users.
    These commands do may not work on external cloud drives (i.e., Google Drive, oneDrive, etc.).

## Introduction
Welcome to the definitive guide on deleting files using the Windows Command Prompt. 
This section is designed to provide you with the necessary command-line skills to 
remove files and directories efficiently. While file deletion is a fundamental 
operation, it's essential to approach it with caution. This guide will not only 
show you how to execute deletions but also how to ensure that you're deleting only 
what you intend to remove, preventing accidental loss of valuable data.

## <b>Open the Command Line</b>
Open the Command Prompt by pressing `Windows Key + R`, typing `cmd`, and pressing 
Enter.

## <b>List Files</b>
List the files in a directory before deletion:

```bash
dir /b
```

## <b>Delete a Single File</b>
!!! warning
    ```
    The following steps deletes your file! Don't use the command if you 
    don't want to delete the file!
    ```
Delete a single file using the `del` command:

```bash
del [filename].txt
```

<i>For example:</i>
```bash
del file.txt
```

## <b>Confirm Deletion</b>
Verify that the file has been deleted:

```bash
dir /b
```

## <b>Delete Multiple Files</b>
!!! warning
    ```
    Warning! The following steps will delete multiple file! Don't use the command 
    if you don't want to delete your files!
    ```
Use wildcards to delete multiple files:

```bash
del *.txt
```

## <b>Delete Files Recursively</b>
!!! warning
    ```
    Warning! The following steps will delete multiple file! Don't use the command 
    if you don't want to delete your files!
    ```
Delete files recursively from subdirectories with the `/s` flag:

```bash
del /s *.txt
```

## <b>Delete Directories</b>
!!! warning
    ```
    Warning! The following steps will delete directories! Don't use the command if 
    you don't want to delete your directories!
    ```
Remove entire directories using `rmdir` or `rd`:

```bash
rmdir /s /q C:\path\to\directory
```

## <b>Secure Deletion</b>
For secure deletion, use a third-party tool like `sdelete` from Sysinternals:

```bash
sdelete -p 3 filename.txt
```

## <b>Empty Recycle Bin</b>
!!! warning
    ```
    Warning! The following steps will empty your recycle bin! Don't use the command 
    if you don't want to empty your recycle bin!
    ```
Empty the recycle bin via the command line:

```bash
rd /s /q C:\$Recycle.Bin
```

## <b>Automate Deletion</b>
Automate the deletion process with a batch script or scheduled task.

## Conclusion
You have now mastered the various methods of deleting files and directories using 
the Command Prompt. While the power to remove data with such efficiency is 
invaluable, always remember the importance of double-checking your commands to 
avoid unintended data loss. These command-line skills will serve you well in 
maintaining a clean and organized digital space, but they come with the 
responsibility to use them wisely and judiciously. As you continue to use these 
commands, you'll develop a keen sense of precision and caution, enhancing your 
overall computing practices.