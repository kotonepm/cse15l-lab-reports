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

---

# Use 2: grep -h

The command display the matched lines of a certain phrase
<br> **Input:** ```grep -h "economic" written_2/non-fiction/OUP/Abernathy/*.txt```
<br> **Output:** 
![Screenshot (64)](https://user-images.githubusercontent.com/103862450/224897135-f58bf0d6-021d-4604-9d7d-e47fca5bb191.png)
<br> 
**Explanation:** Because I wanted to see every time the word "ecnomic" appeared in chapter 1 of the Abernathy text, it highlighted every instance that the word "economic" appeared.
<br> 
<br> **Input:** ```grep -h -c "economic" written_2/non-fiction/OUP/Abernathy/*.txt``` 
<br> **Output:** 
<br> ```5```
<br> ```1```
<br> ```10```
<br> ```2```
<br> ```0```
<br> ```4```
<br> ```0```
<br> ```1```
<br> ```1```
<br> 
**Explanation:** Another cool thing that we can do with the grep -h command is that we can also combine it with the grep -c command to count the instances of a certain phrase in every file.