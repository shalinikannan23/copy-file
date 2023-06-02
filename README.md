# copy-file
## AIM:
To write a python program for copying the contents from one file to another file.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:

from shutil import copy file
### Step 2:

from sys import exit
### Step 3:

Getting input for source file
### Step 4:

Getting input for target file
### Step 5:

Giving condition for files
### Step 6:

Getting statement from the user to print or not want to print

## PROGRAM:
```
#Developed by : Shalini.K
#Register Number: 22008827
import sys
from shutil import copyfile
from sys import exit

source = input("Enter source file with full path:")
target = input("Enter target file with full path:")

# adding exception handling
try:
    copyfile(source, target)
except IOError as e:
    print("Unable to copy file. %s" % e)
    exit(1)
except:
    print("Unexpected error:", sys.exc_info())
    exit(1)
print("\nFile copy done!\n")

while True:
    print("Do you like to print the file ? (y/n): ")
    check = input()
    if check == 'n':
        break
    elif check == 'y':
        file = open(target, "r")
        print("\nHere follows the file content:\n")
        print(file.read())
        file.close()
        print()
        break
    else:
        continue
```

### OUTPUT:
![Screenshot 2023-06-02 203456](https://github.com/shalinikannan23/copy-file/assets/118656529/0c88b24e-c729-4e02-983e-415178f68a36)

![image](https://github.com/shalinikannan23/copy-file/assets/118656529/b3c9a34f-d8ff-428a-ad75-cb202aa53cf1)


## RESULT:
Thus the program is written to copy the contents from one file to another file.
