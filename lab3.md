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
Input: ```find written_2/ -name HandRHawaii.txt ```
<br>
Output: ```written_2/travel_guides/berlitz1/HandRHawaii.txt```
<br>
<br>**Explanation:**

**Use 2:** Search a file with pattern.
<br>
Input: ```find non-fiction/ *.txt```
<br>
Output: 
```non-fiction/```
```non-fiction/OUP
```non-fiction/OUP/Abernathy```
```non-fiction/OUP/Abernathy/ch1.txt```
```non-fiction/OUP/Abernathy/ch14.txt```
```non-fiction/OUP/Abernathy/ch15.txt```
```non-fiction/OUP/Abernathy/ch2.txt```
```non-fiction/OUP/Abernathy/ch3.txt```
```non-fiction/OUP/Abernathy/ch6.txt```
```non-fiction/OUP/Abernathy/ch7.txt```
```non-fiction/OUP/Abernathy/ch8.txt```
```non-fiction/OUP/Abernathy/ch9.txt```
```...```
<br>
<br>
Input: ```find travel_guides/ *.txt```
<br>
Output: 
```travel_guides/```
```travel_guides/berlitz1
```travel_guides/berlitz1/HandRHawaii.txt```
```travel_guides/berlitz1/HandRHongKong.txt```
```travel_guides/berlitz1/HandRIbiza.txt```
```travel_guides/berlitz1/HandRIsrael.txt```
```...```
<br>
<br>**Explanation:**

**Use 3:** How to find and delete a file with confirmation.
<br>
Input: ``` ```
<br>
Output: ``` ```
<br>
<br>
Input: ``` ```
<br>
Output: ``` ```
<br>
<br>**Explanation:**

**Use 4:** Search for empty files and directories.
<br>
Input: ``` ```
<br>
Output: ``` ```
<br>
<br>
Input: ``` ```
<br>
Output: ``` ```
<br>
<br>**Explanation:**
