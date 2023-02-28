# Lab Report 3

---

**About Find:** The find command in UNIX is a command line utility for walking a file hierarchy. It can be used to find files and directories and perform subsequent operations on them. It supports searching by file, folder, name, creation date, modification date, owner and permissions. By using the ‘-exec’ other UNIX commands can be executed on files or folders found. [(https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

---

**Use 1:** Search a file with specific name.
<br>
Input: ```find non-fiction/OUP/Abernathy/ch14.txt```
<br>
Output: ```written_2/non-fiction/OUP/Abernathy/ch1.txt```
<br>
<br>**Explanation:** By adding the full name of the file after the find command in bash, we can find specific names that the user wants to find. This command is useful for user who know that exact file name and want to find the file right away.
<br>
<br>
Input: ```find non-fiction/OUP/Berk/ch1.txt```
<br>
Output: ```non-fiction/OUP/Berk/ch1.txt```
<br>
<br>**Explanation:** In this example, we are demonstrating that this file works for specfic file names. In this example we change the file name to a different file called Berk/ch1.txt and the termainal returned the specific file that we wanted. 

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
<br>**Explanation:** By adding a pattern after using the find command, we can also look for certain patterns in a file. For example, I wanted to find all file that ended in ".txt" in non-fiction.
<br>
<br>
Input: ```find written_2/ -name HandRHawaii.txt```
<br>
Output:```written_2/travel_guides/berlitz1/HandRHawaii.txt```
<br>
<br>**Explanation:** By adding a pattern after using the find command, we can also look for certain patterns in a file. For example, I wanted to find all file that ended in ".txt" in non-fiction.

---

**Use 3:** How to find and delete a file with confirmation.
<br>
Input: ```find non-fiction  -name ch1.txt -exec rm -i {} \;```
<br>
Output: ```rm: remove regular file 'non-fiction/OUP/Abernathy/ch1.txt'?```
<br>
<br>**Explanation:** By adding a pattern after using the find command, we can also look for certain patterns in a file. For example, I wanted to find all file that ended in ".txt" in non-fiction.
<br>
<br>
Input: ```find travel_guides -name HandRHawii.txt -exec rm -i {} \;```
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
<br>**Explanation:** By adding a pattern after using the find command, we can also look for certain patterns in a file. For example, I wanted to find all file that ended in ".txt" in non-fiction.
<br>
<br>
Input: ```find travel_guides -empty```
<br>
Output: ``` ```
<br>
<br>**Explanation:** By adding a "-empty" after using the find command, we can search for empty files and directories. Because every directory that we search for had a file in it, the termainal returned nothing!
