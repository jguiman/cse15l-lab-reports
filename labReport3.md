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
2. The following shows how to get the line number and (# of line being 2 in this case) text before where the target string is found.
<br>
<img width="948" alt="Screen Shot 2022-10-31 at 11 18 10 AM" src="https://user-images.githubusercontent.com/78514873/199080845-27f1367d-b3f5-4bf1-99e8-f596e2aff458.png">

<br>
**Knowing the lines before the target word can help with the users understanding of how a word is being used. In the example above, I wanted to search for pregnant in the context of a woman who is carrying a baby. However, the above example uses it as a figure of speech.**
<br>
#### Get the line number and (#) of text after using: grep -n -A # "Some String" <file1> ... <filen>
<br>
3. The following shows how to get the line number and (# of line being 2 in this case) text after where the target string is found.
<br>

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

