# Troubleshooting

The following table outlines common issues encountered during file operations, possible causes, and the actions you can take to resolve them.

| Symptom | Probable Cause | Action |
|---------|----------------|--------|
| File exists error during move or copy | A file with the same name exists in the destination directory. | Use the move command with an overwrite flag in Windows: ```bash move /Y sourcePath\filename.extension destinationPath\ ``` Or rename the file before moving or copying. |
| Access denied error | Lack of permissions to access the files or directories. | Run the Command Prompt as an administrator, or check and modify the file permissions. |
| Path not found error | The source or destination path does not exist. | Verify that the source and destination paths are correct. Create the directories if they do not exist using: ```bash mkdir pathTo\newDirectory ``` |
| File is in use error | The file you are trying to delete, move, or modify is open in another program. | Close the program that's using the file. If you're not sure which program it is, restart your computer and try the operation again. |
| File is corrupted error | The file cannot be opened because it is corrupted. | Try using file repair tools specific to the file type. If you have a backup, restore the file from the backup. |
| Unable to delete file | The file may be set as read-only or you may not have the necessary permissions. | Check if the file is read-only and change its properties if necessary. Ensure you have the proper permissions to delete the file. |
| File synchronization issues | Files not syncing properly across devices or networks. | Ensure all devices are connected to the network. Check if the sync settings are configured correctly and if there are any error messages, address them as per the application's troubleshooting guide. |

Please replace `sourcePath`, `filename.extension`, and `destinationPath` with your actual file paths and filenames.
