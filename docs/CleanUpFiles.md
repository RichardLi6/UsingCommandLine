# Deleting Files

!!! info
    ```
    These instructions are intended for windows users.
    ```

## <b>Step 1: Open the Command Line</b>
Open the Command Prompt by pressing `Windows Key + R`, typing `cmd`, and pressing Enter.

## <b>Step 2: List Files</b>
List the files in a directory before deletion:

```bash
dir /b
```

## <b>Step 3: Delete a Single File</b>
!!! warning
    ```
    Warning! This step deletes your file! Don't use the command if you don't want to delete the file!
    ```
Delete a single file using the `del` command:

```bash
del [filename].txt
```

<i>For example:</i>
```bash
del file.txt
```

## <b>Step 4: Confirm Deletion</b>
Verify that the file has been deleted:

```bash
dir /b
```

## <b>Step 5: Delete Multiple Files</b>
Use wildcards to delete multiple files:

```bash
del *.txt
```

## <b>Step 6: Delete Files Recursively</b>
Delete files recursively from subdirectories with the `/s` flag:

```bash
del /s *.txt
```

## <b>Step 7: Delete Directories</b>
Remove entire directories using `rmdir` or `rd`:

```bash
rmdir /s /q C:\path\to\directory
```

## <b>Step 8: Secure Deletion</b>
For secure deletion, use a third-party tool like `sdelete` from Sysinternals:

```bash
sdelete -p 3 filename.txt
```

## <b>Step 9: Empty Recycle Bin</b>
Empty the recycle bin via the command line:

```bash
rd /s /q C:\$Recycle.Bin
```

## <b>Step 10: Automate Deletion</b>
Automate the deletion process with a batch script or scheduled task.

