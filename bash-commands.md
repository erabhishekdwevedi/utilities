# Bash Commands

* List Files and Folders
```
ls 
ls -l  //List Detail
ls -a // Hidden
ls xyz*.txt //list filename starts with xyz and of type txt
```

* Opening Directory
```
pwd       // Present working directory
cd ~/    // Access Default Home Directory From Any location
cd ~user2/  // Another User Home Directory
cd -        // Last directory

```


* View content of file 
```
 cat filename
 cat -b filename  // to show line number as well
```

* VI Editor
```
vi filename // it creates the file and opens in shell
i           // Press 'i' to enter editing mode
L           //In edit Mode - Move Cursor Right
H           // In edit Mode - Move Cursor Left
K           // In edit Mode - Move Cursor Upwards
J           // In edit Mode - Move Cursor Downwards
d            // delete character
dd           //delete line


Esc + Esc   // to exit editing mode
:wq         //Write and Quit 
Ctrl + Z    //Exit

```

* Rename
```
 mv oldname newname
```

* Copy file 
```
 cp sourcelocation dir/targetlocation
```
* Delete
```
rm filename
```

* Copy folder from local machine to Remote Machine. Run following command on local.
```
scp fileNameOnLocalMachine root@10.10.10.10:/root/Documents/TargetFolder
```

