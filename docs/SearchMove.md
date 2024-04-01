# Search and Move Files

!!! info
    ```
    These instructions are intended for windows users.
    ```

## <b>Step 1: Open the Command Line</b>
Open the Command Prompt by pressing `Windows Key + R`, typing `cmd`, and pressing Enter.

## <b>Step 2: Search for Files</b>
Use the `dir` command to search for files. 

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

## <b>Step 3: Move the File</b>
Move a file to a new location with the `move` command:

```bash
move C:\[path]\[to]\[source]\[file name].txt C:\[path]\[to]\[destination]\
```
<i>For example</i> To move 'file.txt' from downloads of user Richard to documents:
```
move C:\Users\Richard\Downloads\file.txt C:\Users\Richard\Documents
```

## <b>Step 4: Verify the Move</b>
Check that the file has been moved to the new location:

```bash
dir C:\path\to\destination\
```

## <b>Step 5: Copy the File</b>
Copy a file with the `copy` command:

```bash
copy C:\path\to\source\filename.txt C:\path\to\destination\filename.txt
```

## <b>Step 6: Rename the File</b>
Rename a file using the `ren` or `rename` command:

```bash
ren C:\path\to\filename.txt newfilename.txt
```

## <b>Step 7: Search Within Files</b>
Search for a specific string within files using `findstr`:

```bash
findstr /s "searchstring" *.txt
```

## <b>Step 8: Organize Search Results</b>
Sort the search results by name or date using `dir` with sorting flags:

```bash
dir /b /o:n *.txt
```

## <b>Step 9: Selective Move</b>
Move only certain files using wildcards with `move`:

```bash
move C:\path\to\source\*.txt C:\path\to\destination\
```

## <b>Step 10: Create Directory Structure</b>
Recreate the directory structure in the destination using `xcopy`:

```bash
xcopy /t /e C:\path\to\source\ C:\path\to\destination\
```
