# Organize Files

!!! info
```
These instructions are intended for windows users
```

## <b> Step 1: Open the Command Line </b>
Open the Command Prompt by pressing `Windows Key + R`, typing `cmd`, and pressing `Enter`.

## <b> Step 2: Navigate to Directory </b>
Navigate to your desired directory using the `cd` command. 

```bash
cd [directory address]
```

<i> Example: </i>
```
cd C:\Users\[user]\Documents
```

!!! warning
    you can only change locations properly if you write the full address

    If you do not write the full address, you may need to use cd.. to navigate backwards.

    For example. moving from documents to downloads
    ```
    cd Documents
    cd ..
    cd Downloads
    ``` 
## <b> Step 3: Create a New Directory </b>
Create a new directory using `mkdir`. 

```bash
mkdir [Folder Name]
```

<i> For instance: </i>
```
mkdir NewFolder
```

!!! note

    If you already have a folder with the same file.name in the directory, it will not create a new folder.


## <b> Step 4: Navigate to the New Directory </b>
Change to the newly created directory with `cd`:
```
cd [Folder Name]
```

<i> Example: </i>
```bash
cd NewFolder
```

##  Step 5: Create a New File </b>
Create a new file by using `echo`. 
```
echo. > [file name].txt
```

<i> For example: </i>
```bash
echo. > newfile.txt
```

## Step 6: Open the File
Open the file with a text editor.
```bash
[txt editor] [file name].txt
``` 

<i> For example, </i> use Notepad: 

```bash
notepad newfile.txt
```

<b> ## Step 7: Write Content </b>
Write content to the file using `echo`. 
```
echo [content] >> [file name].txt
```

For instance:
```bash
echo Hello, World! >> newfile.txt
```

## <b>Step 8: Save and Close the File </b>
Save your changes and close the text editor.

## <b> Step 9: Verify the File Content </b>
Verify the file's content with `type`:

```bash
type [filename].txt
```
<i> for example </i>
```bash
type newfile.txt
```
## <b> Step 10: Organizational Tips </b>
Maintain a structured folder hierarchy for better organization and ease of access.

