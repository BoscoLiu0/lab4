# Lab Report 4 - Vim (Week 7)

## 1.Log into ieng6
![image](./Step4.png)
### Key pressed: 
`ssh yal144@ieng6-201.ucsd.edu -> <Enter>`
 This command establishes an SSH connection to the ieng6 server using your username.(Because I set a password in the last lab, I don't need to enter a password to log in)

## 2.Clone your fork of the repository from your Github account (using the SSH URL)
![image](./Step5.png)
### Key pressed: 
`git clone git@github.com:Boscoliu1994/lab7.git -> <Enter>`
Navigate to the directory where I want to clone the repository. Run the  command with the SSH URL of I forked repository-> `Boscoliu1994/lab7.git`

## 3.Run the tests, demonstrating that they fail
![image](./Step6.png)
### Key pressed:
`cd lab7 -> ls -> bash test.sh -> <Enter>`
`cd lab7` Enter the lab7 directory first. `ls` Lists the files and subdirectories in the current directory. `bash test.sh` Run the script file named "test.sh".


## 4.Edit the code file to fix the failing test
![image](./Step7-1.png)
****
![image](./Step7-2.png)
### Key pressed:
`vim ListExample.java -> <Enter> -> Shift + g -> k(6 times) -> e -> x -> i -> 2 -> esc(keyboard) -> :wq -> <Enter>`
Open a Java source code file called "Lisiexample.java" in the `Vim` editor (vim command allows me to edit and modify it). after press `<Enter>`, Vim will launch and open the file, where I can edit.
Press `"Shift + g"` to move the cursor to the last line of the current file - Pressing the `"e"` key will move the cursor to the end of the current word (is 2),The `"x"` key deletes the character where the cursor is located(deleted 2).The `"i"` key switches the editor to insert mode - start typing text at the cursor position and then press 2 to change. `esc` to exit edit->After pressing `":wq"`, Vim will save the currently edited file and exit the editor.

## 5.Run the tests, demonstrating that they now succeed
![image](./Step8.png)
### Key pressed:
`bash test.sh``bash test.sh` Run the script file named "test.sh" again, and get pass the text.

## 6.Commit and push the resulting change to your Github account (you can pick any commit message!)
![image](./Step9-1.png)
****
![image](./Step9-2.png)
### Key pressed:
`git commit ListExamples.java -> <Enter> -> i -> Lab7 test -> esc(keyboard) -> :wq -> <Enter>`
and then `git push git@github.com:Boscoliu1994/lab7.git -> <Enter>`
1.`git commit ListExamples.java`: Commit the file named "ListExamples.java" to my local repository.Press `<Enter>` to confirm submission.Press "i" to enter the insert mode and enter the message `"Lab7 test"` that I submitted.Press the `Esc` key on your keyboard to exit Insert mode and return to normal mode.Enter `:wq` in command line mode to save the file and exit the Vim editor.Press `<Enter>` to exit the Vim editor. 
2. `git push git@github.com: Boscoliu1994 / lab7.git`: this is a git command is used to the change in the local warehouse push (submitted) to a remote warehouse.Press `<Enter>` to confirm push.
