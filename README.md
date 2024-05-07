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
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/2b718e70-b407-4342-ba2c-a44143976cef)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/68ad3808-0735-43a7-aaca-4ec9520ff127)
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/63ac378e-08bd-42e0-87b1-b23499ad75ef)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/b82d7f60-bad1-4b8c-8212-99f5a8d232bf)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/d0cb9b86-f941-4a83-8d0f-b4a9128297d6)
![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/34912c3d-44ca-4387-8e0a-33fffd355985)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/99444324-3e43-4cf8-ad48-330ef0e4835f)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
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

![image](https://github.com/jayavarsha23219/Windows-basic-commands-batchscript/assets/150780319/f2fbc86b-7af0-4d9e-968b-60f1eb6f6d69)


# RESULT:
The commands/batch files are executed successfully.

