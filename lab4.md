# Lab Report 4

---
4. Log into ieng6
![Screenshot (48)](https://user-images.githubusercontent.com/103862450/221757789-e6656427-c1e0-426b-aa22-9b656413d7d2.png)
Because this was my second time logging on to my ieng6 account, the previous commands were saved from the last time. This means that I can sroll through my previous command with the up key and find my username with my ieng6 account attached.
<br> **Keys pressed:** ```<up>``` ```<up>``` ```<ENTER>```

5. Clone your fork of the repository from your Github account
![Screenshot (59)](https://user-images.githubusercontent.com/103862450/221759068-0e26bd1c-df40-4461-81de-6802d0f049ad.png)
To clone a repository from github, we would first go on to the github page that we were given, and click on the fork button. After we fork the respository, there is a drop-down menu, we we click on the green code button. Make sure to copy the ssh link instead of the HTTPS link. After you click on the copy link button go back to the terminal and type is git clone and paste in the ssh link.
<br> **Keys pressed:** ```git clone``` ```<Ctrl> + V``` ```<ENTER>```

6. Run the tests, demonstrating that they fail
![Screenshot (50)](https://user-images.githubusercontent.com/103862450/221758205-998fd6e9-4b72-4c47-8bc3-3950b321605c.png)
By using the lab method, we can auto fill the file names to aviod any errors. We first need to compile the file to see if the tests ran correctly.
<br> **Keys pressed:** ```javac``` ```L <TAB>``` ```T <TAB>``` ```<ENTER>```

7. Edit the code file to fix the failing test
![Screenshot (51)](https://user-images.githubusercontent.com/103862450/221757985-8fbd6a13-caad-48bd-b1a4-5f5b94795867.png)
To edit the code we need to open the a text-editor with the nano command
<br> **Keys pressed:** ```nano``` ```T <TAB>``` ```<ENTER>```
<br>
<br> To get to the specific line that the bug was on, I manually pressed arrow keys to get to the bug in the program. I did not use any commands to get to the specfic line to get the bug.
<br> **Keys pressed:** ```<up>```(42x) ```<right>```(12x)

8. Run the tests, demonstrating that they now succeed
![Screenshot (54)](https://user-images.githubusercontent.com/103862450/221758470-79924a9b-3641-4fc0-81b7-35c04cab3a02.png)
To re-run the tests we also we to re-compile and re-run the tests. Note the the terminal say we need a void main method. This indicates that everythig ran properly.
<br> **Keys pressed:** ```javac``` ```L <TAB>``` ```T <TAB>``` ```<ENTER>``` ```java``` ```L <TAB>``` ```<ENTER>```

9. Commit and push the resulting change to your Github account
![Screenshot (60)](https://user-images.githubusercontent.com/103862450/221758282-1f656452-c987-41a9-8d86-054a59b54f31.png)
To push and commit, we need to enter a bunch of git commands. I tried to press the ```<TAB>``` button for the git command, but it did not work.
<br> **Keys pressed:** ```git add``` ```L <TAB>``` ```<ENTER>``` ```git commit - m"updated"``` ```<ENTER>``` ```git push main origin``` ```<ENTER>```
