# copy-file
## AIM:
To write a python program for copying the contents from one file to another file.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1: from shutil import copy file
### Step 2: from sys import exit
### Step 3: Getting input for source file
### Step 4: Getting input for target file
### Step 5: Giving condition for files
### Step 6: Getting statement from the user to print or not want to print

## PROGRAM:
```
#Developed By:SHALINI.K
#Register No: 212222240095
with open('f1.txt','r') as f1:
    with open ('f2.txt','a') as f2:
        for line in f1:
            f2.write(line)
```
### OUTPUT:
![image](https://github.com/shalinikannan23/copy-file/assets/118656529/68ce94e4-2d53-40e1-ba16-b277c844ec4c)
## RESULT:
Thus the program is written to copy the contents from one file to another file.
