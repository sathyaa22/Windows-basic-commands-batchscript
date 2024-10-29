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
![image](https://github.com/user-attachments/assets/daede906-bc82-433e-83ff-af4e241ec44e)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/b35e1248-de17-4ddc-9f39-e997dda01030)

```
type nul > MyFile.txt
```

![image](https://github.com/user-attachments/assets/9c899fa9-407c-4bf1-9322-0c578b3d3ee7)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/71c2e9fb-53aa-4eb4-9345-0ede32476bcb)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/e3a76feb-b0e9-4f2e-aa66-9903774d2002)


```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/8622257a-bba2-40ee-8e5c-f583202305c5)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```

![image](https://github.com/user-attachments/assets/bbb63bd9-d45c-41f2-b62d-4f6173bbf3a4)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

## COMMAND 

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

![image](https://github.com/user-attachments/assets/93fd8b86-8528-4167-a20b-75e5a54e1978)

## COMMAND

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![image](https://github.com/user-attachments/assets/2c71ced9-6d2e-4bc3-9534-5c8c84d18093)


# RESULT:
The commands/batch files are executed successfully.

