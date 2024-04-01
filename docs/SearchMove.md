# Search and Move Files

## Step 1: Open the Command Line
Open the Command Prompt by pressing `Win + R`, typing `cmd`, and pressing Enter.

## Step 2: Search for Files
Use the `dir` command to search for files. For example, to find all `.txt` files in a directory:

```bash
dir /s /b *.txt
```

## Step 3: Move the File
Move a file to a new location with the `move` command:

```bash
move C:\path\to\source\filename.txt C:\path\to\destination\
```

## Step 4: Verify the Move
Check that the file has been moved to the new location:

```bash
dir C:\path\to\destination\
```

## Step 5: Copy the File
Copy a file with the `copy` command:

```bash
copy C:\path\to\source\filename.txt C:\path\to\destination\filename.txt
```

## Step 6: Rename the File
Rename a file using the `ren` or `rename` command:

```bash
ren C:\path\to\filename.txt newfilename.txt
```

## Step 7: Search Within Files
Search for a specific string within files using `findstr`:

```bash
findstr /s "searchstring" *.txt
```

## Step 8: Organize Search Results
Sort the search results by name or date using `dir` with sorting flags:

```bash
dir /b /o:n *.txt
```

## Step 9: Selective Move
Move only certain files using wildcards with `move`:

```bash
move C:\path\to\source\*.txt C:\path\to\destination\
```

## Step 10: Create Directory Structure
Recreate the directory structure in the destination using `xcopy`:

```bash
xcopy /t /e C:\path\to\source\ C:\path\to\destination\
```
