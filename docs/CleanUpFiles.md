# Deleting Files

## Step 1: Open the Command Line
Open the Command Prompt by pressing `Win + R`, typing `cmd`, and pressing Enter.

## Step 2: List Files
List the files in a directory before deletion:

```bash
dir /b
```

## Step 3: Delete a Single File
Delete a single file using the `del` command:

```bash
del filename.txt
```

## Step 4: Confirm Deletion
Verify that the file has been deleted:

```bash
dir /b
```

## Step 5: Delete Multiple Files
Use wildcards to delete multiple files:

```bash
del *.txt
```

## Step 6: Delete Files Recursively
Delete files recursively from subdirectories with the `/s` flag:

```bash
del /s *.txt
```

## Step 7: Delete Directories
Remove entire directories using `rmdir` or `rd`:

```bash
rmdir /s /q C:\path\to\directory
```

## Step 8: Secure Deletion
For secure deletion, use a third-party tool like `sdelete` from Sysinternals:

```bash
sdelete -p 3 filename.txt
```

## Step 9: Empty Recycle Bin
Empty the recycle bin via the command line:

```bash
rd /s /q C:\$Recycle.Bin
```

## Step 10: Automate Deletion
Automate the deletion process with a batch script or scheduled task.

