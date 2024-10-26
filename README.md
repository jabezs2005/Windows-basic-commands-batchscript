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
### Create a directory named "MyLab" on the desktop.
![1](https://github.com/user-attachments/assets/03055dd2-e2b2-4198-9eed-9cdeb3d705fb)

## COMMAND AND OUTPUT
### mkdir %userprofile%\Desktop\MyLab
![2](https://github.com/user-attachments/assets/13436144-37cf-4656-a5d3-fd2f6b6a6c27)
![3](https://github.com/user-attachments/assets/ffb748ef-fe8f-4437-8eb3-44b5f988a33d)
### Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT
### cd %userprofile%\Desktop\MyLab
![4](https://github.com/user-attachments/assets/ae4dd7d9-3de7-4909-83c9-fc6516ddec88)
![5](https://github.com/user-attachments/assets/89c8afef-8fbc-4dc0-9fb1-ae8f43e902f5)

### List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
### dir %userprofile%\Desktop\MyLab
![6](https://github.com/user-attachments/assets/27d1302f-9fab-43a5-909e-596bd284a65d)
![7](https://github.com/user-attachments/assets/7b4dfd2d-4e75-431e-a6bf-8f666739bdfb)
### Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT
### mkdir %userprofile%\Desktop\Backup

### copy MyFile.txt %userprofile%\Desktop\Backup
![8](https://github.com/user-attachments/assets/01be8dee-f051-4e07-a60a-b690c151521b)

### Move the "MyLab" directory to the "Documents" folder.

![9](https://github.com/user-attachments/assets/1d40d86d-19f5-4ca7-95be-faf22dd17c25)
## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
### Exercise 2: Advanced Batch Scripting
### Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
### Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
### OUTPUT
![10](https://github.com/user-attachments/assets/1196d074-f0ac-4930-8814-8fba0ade2f1e)
### RESULT:
The commands/batch files are executed successfully.

