# Troubleshooting

The following table outlines common issues encountered during file operations, possible causes, and the actions you can take to resolve them.

| Symptom | Probable Cause | Action |
|---------|----------------|--------|
| File exists error during move or copy | A file with the same name exists in the destination directory. | Use the move command with an overwrite flag in Windows: ```bash move /Y sourcePath\filename.extension destinationPath\ ``` Or rename the file before moving or copying. |
| Access denied error | Lack of permissions to access the files or directories. | Run the Command Prompt as an administrator, or check and modify the file permissions. |
| Path not found error | The source or destination path does not exist. | Verify that the source and destination paths are correct. Create the directories if they do not exist using: ```bash mkdir pathTo\newDirectory ``` |

Please replace `sourcePath`, `filename.extension`, and `destinationPath` with your actual file paths and filenames.
