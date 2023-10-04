# Remote Access and FileSystem (Week 1)
In this lab report, I use the lecture1 folder provided as my example. The circled numbers in each image corresponds to the numbered finding in each cd, ls, and cat category.
## cd command
1. Calling the command 'cd' with no arguments returns nothing. The current working directory when this command was run is nothing. Because  no arguments were included as a directory, the command returns nothing, which is the expected output.
2. Calling the command 'cd' with 'lecture1' as its argument changes the directory of the file and accesses the lecture1 folder.
Output: [user@sahara ~/lecture1]$
This is expected as cd is supposed to go into the directory its argument assigns (if it's the subsequential directory after the previous). Therefore, it is not an error.
3. Calling the command 'cd' with the file 'en-au.txt' as its argument produces an error because the command isn't meant to access files.
![Image](lab1_cd_examples.png)

## ls command
1. Calling the command 'ls' with no arguments returns 'lecture1' which is the name of the folder in the current directory.
2. Calling the command 'ls' with 'lecture1' as its argument returns the contents in the lecture1 folder, both files and folders.
3. Calling the command 'ls' with the file 'en-au.txt' as its argument produces an error and is unable to access the file because the ls command isn't meant to access files.

## cat command
1. Calling the command 'cat' with no arguments copies whatever is typed and entered into the terminal, creating a clone of the message inputed.
