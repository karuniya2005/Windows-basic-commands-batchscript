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

![328033026-8a9702bd-2318-4936-90c0-b956172a38ac](https://github.com/vinothmp21102005/Windows-basic-commands-batchscript/assets/145972215/36607372-eb05-4786-b88b-7d1051e59e63)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![328033073-28ea7dc9-de64-49b2-9b17-018350fd5af3](https://github.com/vinothmp21102005/Windows-basic-commands-batchscript/assets/145972215/b03c876a-e821-40e0-a260-6c63d04a6810)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![328033145-8fba2968-e4ef-46c6-a0ad-73055970cfaf](https://github.com/vinothmp21102005/Windows-basic-commands-batchscript/assets/145972215/d9cecd51-e460-469f-bc89-30551d1cdab8)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![328033184-43dd0eb7-9d30-4fa5-b744-72ce1041d368](https://github.com/vinothmp21102005/Windows-basic-commands-batchscript/assets/145972215/29a2c9b4-cfff-4ead-80c0-86e55524218c)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![328033233-11a3d6f1-3612-4b94-bca3-927e98bd9bf0](https://github.com/vinothmp21102005/Windows-basic-commands-batchscript/assets/145972215/fef9a864-7fea-4fc5-bc21-e3d2f3c5d776)


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


![328033316-ab6810ef-9e2b-4d14-80ba-6ee42c8d78b2](https://github.com/vinothmp21102005/Windows-basic-commands-batchscript/assets/145972215/ee69dc2c-26a4-44f9-a376-178edb1903a4)



# RESULT:
The commands/batch files are executed successfully.

