# Delete Files


!!! info
    These instructions are intended for windows users.

    These commands do may not work on external cloud drives (i.e., Google Drive, oneDrive, etc.).

    User is expected to have files and directories to delete for this section.

<b>Introduction</b> 

The following is the guide on deleting files using the Windows Command Prompt. This section is meticulously designed to provide you with the necessary command-line skills to remove files and directories efficiently. While file deletion is a fundamental operation, it's essential to approach it with caution. This guide will not only show you how to execute deletions but also how to ensure that you're deleting only what you intend to remove, preventing accidental loss of valuable data.

1. Open the Command Prompt by pressing `Windows Key + R`, typing `cmd`, and pressing 
Enter. 

    <figure markdown="span">
    ![Command Prompt](./CommandLine.png){ height="800"}
    <figcaption>Command Prompt window</figcaption>
    </figure>

2. Find the file, if you know the directory of the file already, you can move to step 4.

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

3. Copy the file location of the address by highlighting the directory using ctrl + c.

    For example if I'm looking for the txt file, only copy the address before the file.
    ```
    C:\Users\Richard\Downloads\text.txt
    ```
    I would only copy the bottom portion.
    ```
    C:\Users\Richard\Downloads\
    ```


4. Navigate to your desired file location using the `cd` command where you want to delete files.

    ```
    cd [directory address]
    ```

    <i> For Example: </i>
    ```bash
    cd C:\[Users]\[user]\Documents
    ```

5. List the files in a directory before deletion: 
    ```bash
    dir /b
    ```



6. Delete a single file using the `del` command: 
    !!! warning
        The following steps deletes your file! Don't use the command if you 
        don't want to delete the file!
        
    ```bash
    del [filename].txt
    ```

    <i>For example:</i>
    ```bash
    del file.txt
    ```

7. Verify that the file has been deleted:

    ```bash
    dir /b
    ```

8. Use wildcards to delete multiple files:

    !!! warning
        The following steps will delete multiple file! Don't use the command 
        if you don't want to delete your files!


    ```bash
    del *.txt
    ```

9. Remove entire directories using `rmdir` or `rd`: 

    !!! warning
        The following steps will delete directories! Don't use the command if 
        you don't want to delete your directories!


    ```bash
    rmdir /s /q C:\path\to\directory
    ```

10. Secure deletion, we are use a third-party tool like `sdelete` from Sysinternals: 

    ```bash
    sdelete -p 3 filename.txt
    ```

11. Empty the recycle bin via the command line: 

    !!! warning
        The following steps will empty your recycle bin! Don't use the command 
        if you don't want to empty your recycle bin!

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