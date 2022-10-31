# Lab Report #3
<br>
## 3 Alternative Ways to use the grep Command
<br>
### Method 1: Find the exact target string with the target not just being a substring.
<br>
#### Use: grep -w "some string" <file 1> ... <>
<br>
1.
<br>
2.
<br>
3.
<br>
### Method 2: Getting the line number of the string found and to read lines before/after.
<br>
#### Get the line number using: grep -n "Some String" <file1> ... <filen>
<br>
1. The following is how to get the line numbers of how to get the line number of the string found from a file(s).
<br>
<img width="834" alt="Screen Shot 2022-10-31 at 10 59 47 AM" src="https://user-images.githubusercontent.com/78514873/199078806-2cb7839c-6eb7-44af-8877-244568db54da.png">

<br>
**Knowing the line numbers of where the text is found is important because it will give the user a sense of where exactly it is located in a file and also helps with additional options such as -A and -B. which prints out lines before and after the target.**
<br>
#### Get the line number and (#) of text before using: grep -n -B # "Some String" <file1> ... <filen>
<br>
2. The following shows how to get the line number and text before where the target string is found.
<br>
3.
<br>
### Method 3: Read lines found before/after target string is found.
<br>
<br>
1.
<br>
2.
<br>
3.
<br>

