# Lab Report 5

---

**About Grep:** The grep filter searches a file for a particular pattern of characters, and displays all lines that contain that pattern. The pattern that is searched in the file is referred to as the regular expression (grep stands for global search for regular expression and print out). [(https://www.geeksforgeeks.org/grep-command-in-unixlinux/)](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

# Use 1: grep -c

The command grep -c will count how many time a certain phrase is repeated in the file
<br> **Input:** ```grep -c "Japan" written_2/travel_guides/berlitz1/IntroJapan.txt```
<br> **Output:** ```50```
<br> 
<br> **Explanation:** Because the phrase Japan is found 50 times in the file, the termainal returns 50.
<br> 
<br> **Input:** ```grep -c "New York" written_2/travel_guides/berlitz1/IntroJapan.txt```
<br> **Output:** ```0```
<br> 
<br> **Explanation:** Because the phrase New York is not found in the file, the termainal returns 0.
<br> 
---

#Use 2: grep -

