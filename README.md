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
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/02cb9e56-daef-49d0-ba44-12403dc0c941)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/630d8c45-4dbc-409a-8d52-fb0c1f9f8fb1)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/1dd80b8b-3cd5-4add-903a-cec1a1b0a670)



## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/553ed90c-9e84-4f6f-9b84-2b59db4aaa09)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/67837965-d7cf-40dc-aa57-94cc53b6e68f)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```@echo off
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
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/bbfdf048-d358-4f79-8ed5-d421cde8ae50)





# RESULT:
The commands/batch files are executed successfully.

