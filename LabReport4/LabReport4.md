## Lab Report 4  
It took me about 10 minutes according to the timer.  
  
### Step 4: Log into ieng6  
To begin, I wanted to log into the ieng6. In the terminal, I typed in `s` `s` `h` `<Space>` `c` `s` `1` `5` `l` `f` `a` `2` `3` `f` `k` `@` `i` `e` `n` `g` `6` `.` `u` `c` `s` `d` `.` `e` `d` `u` and pressed `<Enter>` to log into ieng6. After a little bit, it automatically loggged me in without requiring a password.
  
![Image](lab4_login.png)  

### Step 5: Clone your fork of the repository from your Github account (using the SSH URL)  
Next, I cloned a fork of my repository and copied the ssh link by clicking the clipboard. Then in my terminal, I typed in `g` `i` `t` `<Space>` `c` `l` `o` `n` `e` `<Space>` `Cmd+V` which pasted the ssh link `git@github.com:iccxu/lab7.git`. Then I pressed `<Enter>` into the terminal to finalize the command and it began cloning into my ieng6 account.  
  
![Image](lab4_clone.png)  

### Step 6: Run the tests, demonstrating that they fail  
Afterwards, I typed `c` `d` `<Space>` `l` `a` `b` `7` `<Enter>` to get into the directory of the lab7 file. Then I typed `b` `a` `s` `h` `<Space>` `t` `e` `s` `t` `.` `s` `h` `<Enter>` which bash allows us to run the tests of the ListExamples files based on the commands in `test.sh`. Upon doing so, I received a failure of one of the tests.  
  
![Image](lab4_failed_test.png)  
  
** Note: I will begin to put words into one code block chunk but they still refer to the format of individual key presses. For example: `vim` = `v` `i` `m`.
### Step 7: Edit the code file to fix the failing test  
I started off by fixing the `ListExamples.java` file. To fix the code, I entered vim mode by typing `vim` `<Space>` `ListExamples.java` `<Enter>`. Then I typed `/` `index1` `<Enter>` to search for the first occurrence of `index1` in the code and then pressed `<Enter>`. Afterwards, I kept pressing `n` until I reached the last while loop. Then I pressed `i` to enter insert mode and I pressed the `<Right>` key 6 times until I reached the end of `index1`. Then, `<Backspace>` `2` `<Esc>` `:` `w` `<Enter>` to change `index1` to `index2` and saved the file by typing `:` `w` `<Enter>` command in vim.  
  
![Image](lab4_codefix.png)  

### Step 8: Run the tests, demonstrating that they now succeed  
After I finished fixing the bugs, I ran `bash test.sh` once again to quickly run the commands of compiling and running JUnit by typing `bash` `<Space>` `test.sh` `<Enter>` and all the tests passed.  
  
![Image](lab4_fixed_test.png)  

### Step 9: Commit and push the resulting change to your Github account (you can pick any commit message!)  
Afterwards, I typed in `git` `<Space>` `add` `<Space>` `ListExamples.java` `<Enter>` to add the file to my workspace. Then `git` `<Space>` `status` `<Enter>` to see what was in the current workspace of files waiting to get pushed into the Github server. I then typed in `git` `<Space>` `commit` `<Enter>` to commit the changes and added a message. Once I finished, I typed in `:` `w` `q` `<Enter>` to save and quit the changes of my commit message then `git` `<Space>` `push` `<Enter>` to push the file into the GitHub server.  
![Image](lab4push.png)  

