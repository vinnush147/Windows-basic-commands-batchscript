# Windows-basic-commands-batchscript
EX08 Windows-basic-commands-batchscript

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


## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Meyyappan-T/Windows-basic-commands-batchscript/assets/128804366/2d4f79b9-b78b-4f2c-bf06-095af7642d40)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT:
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Meyyappan-T/Windows-basic-commands-batchscript/assets/128804366/bbadcf18-2ce4-4c5d-a2b9-567e61f9c906)


```
type nul > MyFile.txt
```

![image](https://github.com/Meyyappan-T/Windows-basic-commands-batchscript/assets/128804366/6754bdb8-cd39-4007-8dbc-52a8dfb616de)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT:
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Meyyappan-T/Windows-basic-commands-batchscript/assets/128804366/54a3204d-1415-409f-9498-a55cdf34b56d)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/Meyyappan-T/Windows-basic-commands-batchscript/assets/128804366/63b4bec5-7694-456f-9745-ebeef64af7d9)


```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/Meyyappan-T/Windows-basic-commands-batchscript/assets/128804366/c1cce673-92e2-4e4b-b8e8-bb73c553479a)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![image](https://github.com/Meyyappan-T/Windows-basic-commands-batchscript/assets/128804366/d617b586-645a-4c52-837f-d8a6b0a1d0a8)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.




## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```


## OUTPUT:
![image](https://github.com/Meyyappan-T/Windows-basic-commands-batchscript/assets/128804366/5b056a85-f3c1-4139-8603-8eba276d227c)


## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT:
![image](https://github.com/Meyyappan-T/Windows-basic-commands-batchscript/assets/128804366/784daff7-4c23-494d-bd68-a98bd055c0cf)


# RESULT:
The commands/batch files are executed successfully.
