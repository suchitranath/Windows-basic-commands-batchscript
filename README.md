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
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/20042f0a-2994-4956-a2c7-ad1744f94c1a)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/3e71ee19-ab89-46f5-8f11-ea6531c0816f)
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/3a04e79b-42d5-4296-a26d-367ec793e995)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/3960e8eb-94b7-427e-937c-a85cfb07ef21)


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/4bc34af7-dc58-4f7b-8fbd-512f0c68260b)

![image](https://github.com/suchitranath/Windows-basic-commands-batchscript/assets/145742631/9b2530aa-fb1d-4fa6-b329-73c34601e5a9)

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

