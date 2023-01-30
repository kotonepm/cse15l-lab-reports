# Hello, World! Welcome to CSE 15L

**Installing VScode**
1. Go to the Visual Studio Code website [(https://code.visualstudio.com/)](https://code.visualstudio.com/).
2. At the top right, you will see a button where you can download VScode. Make sure to select the correct version that you need.
3. Run the installer and follow the prompted instructions to install VScode. 

*Your screen should look like this when VScode is succeesfully installed:*
![Screenshot (25)](https://user-images.githubusercontent.com/103862450/212399123-96191e29-dcbe-4543-a6d8-7ae23d103ba8.png)

---

**Remotely Connecting**
1. After successfully installing VScode, locate the termainal at the top left of the screen. Click on termainal to open the terminal.
2. After the termianl is open, click on the termainal and enter the following: `ssh cs15lwi23[Name]@ieng6.ucsd.edu.` Replace [Name] with your own 3-letter ID.              *(Note: if this is your first time logging on to the server you will be prompted with a yes or no question. Type Yes into the termainal and press **ENTER**)*
3. Type in the password you made on the [CSE 15L Webstie](https://sdacs.ucsd.edu/~icc/index.php) and press **ENTER**.                                                      *(Note: When typing in the passward, the cursor **will not** move. This is normal so don't panic)*

*Your screen should look like this when you have successfully connnected:*
![Screenshot (27)](https://user-images.githubusercontent.com/103862450/212399191-4a113800-0ac5-4059-80a7-423fd9046a96.png)

---

**Trying Some Commands**
1. Now that you have successfully logged on the server, try running some commands both on your terminal after you log in, and before entering your **ssh**.
2. Try running each of these commands in the terminal and see what they do. To run a command, simply type in one of the commands in your terminal and press **ENTER**.
* `cd ~`
* `cd`
* `ls -lat`
* `ls -a`
* `ls` <directory> where `<directory>` is `/home/linux/ieng6/cs15lwi23/cs15lwi23[NAME]` *(Replace [Name] with one of the other group members’ username)*
* `cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/`
* `cat /home/linux/ieng6/cs15lwi23/public/hello.txt`

*These are some example of commands that have been run on the terminal:*
![Screenshot (28)](https://user-images.githubusercontent.com/103862450/212399055-0ef7c863-f0c0-485b-b78d-a8d215e1dd27.png)
 
 **Here's what some of these commands do:**
  
3. You now have VScode installed and a basic understanding of running commands in the terminal! To log off, enter one of the following commands:
* Ctrl-D
* Run the command **exit**
