# Remote Access and FileSystem (Week 1)
In this lab report, I use the lecture1 folder provided as my example. The circled numbers in each image corresponds to the numbered finding in each cd, ls, and cat category.
## cd command
1. Calling the command 'cd' with no arguments returns nothing. This isn't an error as the directory is blank, hence returning nothing.
2. Calling the command 'cd' with 'lecture1' as its argument changes the directory of the file and accesses the lecture1 folder.
3. Calling the command 'cd' with the file 'en-au.txt' as its argument produces an error because the command isn't meant to access files.
![Image](lab1_cd_examples.png)

## ls command
1. Calling the command 'ls' with no arguments returns 'lecture1' which is the name of the folder in the current directory.
2. Calling the command 'ls' with 'lecture1' as its argument returns the contents in the lecture1 folder, both files and folders.
3. Calling the command 'ls' with the file 'en-au.txt' as its argument produces an error and is unable to access the file because the ls command isn't meant to access files.

## cat command
1. Calling the command 'cat' with no arguments copies whatever is typed and entered into the terminal, creating a clone of the message inputed.
