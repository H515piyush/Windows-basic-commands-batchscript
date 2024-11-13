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
~~~
mkdir %userprofile%\Desktop\MyLab
~~~
![325093274-30906be8-14a0-42df-be77-32fd1db31b60](https://github.com/user-attachments/assets/5f92b45a-3498-4077-879e-cbb5012c8c90)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
~~~
cd %userprofile%\Desktop\MyLab
~~~
![325093472-219b74d7-05db-4607-ba11-27751dc8e214](https://github.com/user-attachments/assets/cbd742e2-2bcc-4f5f-9cd9-a5b1c51e0f20)
![325093753-231c6c4e-3340-415c-953c-3d929983c9ef](https://github.com/user-attachments/assets/2b057e7a-f148-4d81-9c41-d744eed444f3)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
~~~
dir %userprofile%\Desktop\MyLab
~~~
![325094082-26b5dd3d-0930-4a7b-bbc1-b70d2eab433d](https://github.com/user-attachments/assets/29631b2b-b995-440a-ad2b-f6a14f31e938)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
~~~
![325095313-4b522d08-477a-4ac2-bdf8-ce34b5377f8a](https://github.com/user-attachments/assets/800b1dd5-9005-455b-9ed8-9af2d433fcbb)
![325095614-2b3d2723-ef8d-47a6-a7a6-d230fc1e3937](https://github.com/user-attachments/assets/263a2e69-a5cb-4ba8-8ac0-ccd24d97323f)



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
~~~
mv Myfile.txt %userprofile%\Documents
~~~

![325095890-7a71bbce-a804-472a-96be-308a5862f6ba](https://github.com/user-attachments/assets/54a2165c-de39-4ef4-bea8-33622ef16353)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
~~~
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
~~~
## OUTPUT

![325099134-3d062ebb-7d20-4c09-95dc-b10861f34223](https://github.com/user-attachments/assets/5e789d5b-8f70-403a-8bf5-2f7f036dd789)





# RESULT:
The commands/batch files are executed successfully.

