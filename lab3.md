# Lab Report 2

**About Find:** The find command in UNIX is a command line utility for walking a file hierarchy. It can be used to find files and directories and perform subsequent operations on them. It supports searching by file, folder, name, creation date, modification date, owner and permissions. By using the ‘-exec’ other UNIX commands can be executed on files or folders found. 

**Use 1:** Search a file with specific name.
<br>
Input: ```find written_2/ -name ch1.txt```
<br>
Output: 
<br>```written_2/non-fiction/OUP/Abernathy/ch1.txt```
<br>```written_2/non-fiction/OUP/Berk/ch1.txt```
<br>```written_2/non-fiction/OUP/Fletcher/ch1.txt```
<br>```written_2/non-fiction/OUP/Kauffman/ch1.txt```
<br>```written_2/non-fiction/OUP/Rybczynski/ch1.txt ```
<br>
<br>
Input: ```find written_2/ -name HandRHawaii.txt```
<br>
Output: ```written_2/travel_guides/berlitz1/HandRHawaii.txt```
<br>
<br>**Explanation:**

**Use 2:** Search a file with pattern.
<br>
Input: ```find non-fiction/ *.txt```
<br>
Output:
<br>```non-fiction/```
<br>```non-fiction/OUP```
<br>```non-fiction/OUP/Abernathy```
<br>```non-fiction/OUP/Abernathy/ch1.txt```
<br>```non-fiction/OUP/Abernathy/ch14.txt```
<br>```(more code below)```
<br>
<br>
Input: ```find travel_guides/ *.txt```
<br>
Output:
<br>```travel_guides/```
<br>```travel_guides/berlitz1```
<br>```travel_guides/berlitz1/HandRHawaii.txt```
<br>```travel_guides/berlitz1/HandRHongKong.txt```
<br>```travel_guides/berlitz1/HandRIbiza.txt```
<br>```(more code below)```
<br>
<br>**Explanation:**

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
<br>**Explanation:**

**Use 4:** Search for empty files and directories.
<br>
Input: ```find non-fiction  -empty```
<br>
Output: ```find travel_guides -empty```
<br>
<br>
Input: ``` ```
<br>
Output: ``` ```
<br>
<br>**Explanation:**
