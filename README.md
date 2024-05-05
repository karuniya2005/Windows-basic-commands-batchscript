# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 


# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab

![Screenshot 2024-05-05 220006](https://github.com/karuniya2005/Windows-basic-commands-batchscript/assets/161425769/8a9702bd-2318-4936-90c0-b956172a38ac)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![Screenshot 2024-05-05 220053](https://github.com/karuniya2005/Windows-basic-commands-batchscript/assets/161425769/28ea7dc9-de64-49b2-9b17-018350fd5af3)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![Screenshot 2024-05-05 220206](https://github.com/karuniya2005/Windows-basic-commands-batchscript/assets/161425769/8fba2968-e4ef-46c6-a0ad-73055970cfaf)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![Screenshot 2024-05-05 220256](https://github.com/karuniya2005/Windows-basic-commands-batchscript/assets/161425769/43dd0eb7-9d30-4fa5-b744-72ce1041d368)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![Screenshot 2024-05-05 220335](https://github.com/karuniya2005/Windows-basic-commands-batchscript/assets/161425769/11a3d6f1-3612-4b94-bca3-927e98bd9bf0)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![Screenshot 2024-05-05 220450](https://github.com/karuniya2005/Windows-basic-commands-batchscript/assets/161425769/ab6810ef-9e2b-4d14-80ba-6ee42c8d78b2)


# RESULT:
The commands/batch files are executed successfully.

