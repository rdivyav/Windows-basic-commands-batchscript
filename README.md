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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

mkdir %userprofile%\Desktop\MyLab


![image](https://github.com/rdivyav/Windows-basic-commands-batchscript/assets/148604723/87d67fab-8005-4543-a6ec-bb37b624c618)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.

cd %userprofile%\Desktop\MyLab

![image](https://github.com/rdivyav/Windows-basic-commands-batchscript/assets/148604723/14e96613-d109-4979-b738-34b6338ece83)


![image](https://github.com/rdivyav/Windows-basic-commands-batchscript/assets/148604723/82b1d36f-8660-49d0-bf97-20a1c2d1ab1c)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

dir %userprofile%\Desktop\MyLab


![image](https://github.com/rdivyav/Windows-basic-commands-batchscript/assets/148604723/800b5913-8d9e-4250-a72f-775653e4643f)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

mkdir %userprofile%\Desktop\Backup


copy MyFile.txt %userprofile%\Desktop\Backup


![image](https://github.com/rdivyav/Windows-basic-commands-batchscript/assets/148604723/22cff166-c137-4462-85f8-eba660c2195a)


![image](https://github.com/rdivyav/Windows-basic-commands-batchscript/assets/148604723/46582502-affe-4d09-a5db-a5aa7e625415)

## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents


![image](https://github.com/rdivyav/Windows-basic-commands-batchscript/assets/148604723/f5e2647b-b082-4917-b72d-2f0942027edc)

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

![image](https://github.com/rdivyav/Windows-basic-commands-batchscript/assets/148604723/619933b3-1809-4adb-83fa-162050f8a37c)

# RESULT:
The commands/batch files are executed successfully.

