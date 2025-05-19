# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "my-lab"

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/b6632b84-b38d-4f91-87bd-3d975b0b73f9)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/196422ac-e64d-4b6b-a1eb-9778cd7df113)

type nul > MyFile.txt

![image](https://github.com/user-attachments/assets/84e4dedb-5fb3-4d73-a25e-345746f78471)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/a25b176d-5204-4e20-a4a4-b209fe0360b9)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/33959722-dd70-47b1-acc7-68c16a3bf799)

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/user-attachments/assets/fae04cfc-64fb-429c-bf8b-e29851e455a1)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
```
move MyLab Documents

![image](https://github.com/user-attachments/assets/5f9ffad7-97b9-466d-a05e-deca5c5f1335)

## Exercise 2: Advanced Batch Scripting
Create a batch file named on the desktop. The batch file need to have a variable assigned with a desired name for ex. name="John" and display as "Hello, John".
<h2>Command</h2>

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

![image](https://github.com/user-attachments/assets/06dc3e22-f3d1-4612-9008-ea761922ac7e)

<h2>Command</h2>

```
  @echo off
  mkdir %userprofile%\Desktop\DocBackup
  copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
  del %userprofile%\Documents\*.docx
  echo Backup and deletion completed successfully!
```

## OUTPUT

![image](https://github.com/user-attachments/assets/229e26b4-f89c-48be-91e5-cefccdecbeb8)

# RESULT:
The commands/batch files are executed successfully.

