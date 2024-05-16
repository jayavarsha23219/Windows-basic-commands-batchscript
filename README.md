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

### DEVELOPED BY : JAYAVARSHA T
### REGISTER NUMBER : 21223040075


# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/91986771-21b4-4fd8-b052-e9c8eaa022b3)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/97209073-b009-4638-b064-9b1faefa543a)
```
type nul > MyFile.txt
```
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/3d6f382a-2b9e-48cc-9360-2a1e6349039f)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/9e58bbfb-e190-4bb9-9d33-247766ee242f)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/df143685-d97f-4cc1-907b-16634b280da3)
```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/61f3d94c-e7c5-4b0c-8322-716dba860f6a)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/0ab68368-edd3-4980-812f-1ccbd07a1766)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/e4344e73-1bce-4fa9-9d33-92032f165454)

## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/28b4318f-3b6b-4f83-981d-67fc87fe331f)

# RESULT:
The commands/batch files are executed successfully.

