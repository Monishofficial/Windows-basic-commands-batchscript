## NAME: MONISH N
## REG NO:212223240097
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
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Monishofficial/Windows-basic-commands-batchscript/assets/149455421/59c90704-5b12-4177-a77a-7ba7090a4a2f)
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Monishofficial/Windows-basic-commands-batchscript/assets/149455421/a0ec5224-4d03-4f32-8c12-a0cd113415a9)
![image](https://github.com/Monishofficial/Windows-basic-commands-batchscript/assets/149455421/aa76fc59-7635-41c0-a385-6fd20474b201)
List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Monishofficial/Windows-basic-commands-batchscript/assets/149455421/1f2b2e6b-0a07-4323-800d-0919d9dbbfb3)
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/Monishofficial/Windows-basic-commands-batchscript/assets/149455421/56cf387d-391f-4ee3-a37a-e5936aff4c86)

![image](https://github.com/Monishofficial/Windows-basic-commands-batchscript/assets/149455421/03d67c90-b4bb-4c6d-b7b6-21bb5eb4c5c8)
Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/Monishofficial/Windows-basic-commands-batchscript/assets/149455421/69e40cef-df3b-45cd-83d3-5d7619c16a17)
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
![image](https://github.com/Monishofficial/Windows-basic-commands-batchscript/assets/149455421/c7527a13-d1ed-4ae0-ae32-4a8b35279a19)

# RESULT:
The commands/batch files are executed successfully.

