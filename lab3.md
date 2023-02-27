# Lab Report 3

---

**About Find:** The find command in UNIX is a command line utility for walking a file hierarchy. It can be used to find files and directories and perform subsequent operations on them. It supports searching by file, folder, name, creation date, modification date, owner and permissions. By using the ‘-exec’ other UNIX commands can be executed on files or folders found. [(https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

---

**Use 1:** Search a file with specific name.
<br>
Input: ```find non-fiction/OUP/Berk/ch1.txt```
<br>
Output: ```non-fiction/OUP/Berk/ch1.txt```
<br>
<br>
<br>
Input: ```find non-fiction/OUP/Abernathy/ch14.txt```
<br>
Output: ```written_2/non-fiction/OUP/Abernathy/ch1.txt```
<br>
<br>**Explanation:** By adding a file name after the find command in bash, we can find files or all files that have the same name. For example, in the first input and output, I wanted to find all files that had "ch1.txt" , which returned multiple file, and in the second input and output, because only one file had "HandRHawaii.txt" in it only one file returned. 

---

**Use 2:** Search a file with pattern.
<br>
Input: ```find written_2/ -name ch1.txt```
<br>
Output:
<br>```written_2/non-fiction/OUP/Abernathy/ch1.txt```
<br>```written_2/non-fiction/OUP/Berk/ch1.txt```
<br>```written_2/non-fiction/OUP/Berk/ch1.txt```
<br>```written_2/non-fiction/OUP/Fletcher/ch1.txt```
<br>```written_2/non-fiction/OUP/Kauffman/ch1.txt```
<br>```written_2/non-fiction/OUP/Rybczynski/ch1.txt```
<br>
<br>
Input: ```find written_2/ -name HandRHawaii.txt```
<br>
Output:```written_2/travel_guides/berlitz1/HandRHawaii.txt```
<br>
<br>**Explanation:** By adding a pattern after using the find command, we can also look for certain patterns in a file. For example, I wanted to find all file that ended in ".txt" in non-fiction and travel_guides so the terminal return every single file that had ".txt" at the end.

---

**Use 3:** How to find and delete a file with confirmation.
<br>
Input: ```find non-fiction  -name ch1.txt -exec rm -i {} \;```
<br>
Output: ```rm: remove regular file 'non-fiction/OUP/Abernathy/ch1.txt'?```
<br>
<br>
Input: ```find travel_guides  -name HandRHawii.txt -exec rm -i {} \;```
<br>
Output: ``` ```
<br>
<br>**Explanation:** By adding a ```-exec rm -i {} \;``` after using the find command, we can delete files in a directory. For the first example, because there were more that one file that conatined "ch1.txt" at the end, it returned a prompt that asked if the user wanted to delete the file, unlike the second example which only had one unique file that ended with "HandRHawii.txt". 

---

**Use 4:** Search for empty files and directories.
<br>
Input: ```find non-fiction -empty```
<br>
Output: ``` ```
<br>
<br>
Input: ```find travel_guides -empty```
<br>
Output: ``` ```
<br>
<br>**Explanation:** By adding a "-empty" after using the find command, we can search for empty files and directories. Because every directory that we search for had a file in it, the termainal returned nothing!
