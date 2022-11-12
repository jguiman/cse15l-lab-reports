# Lab Report #3
<br>
## 3 Alternative Ways to use the grep Command
<br>
### Method 1: Find the exact target string with the target not just being a substring.
<br>
#### Use: grep -w "some string" <file 1> ... <>
<br>
Example 1: searching for men
<br>
Command: grep -w "men" */*.txt
<br>
**Output:**
<br>
<img width="1128" alt="Screen Shot 2022-10-31 at 11 36 37 AM" src="https://user-images.githubusercontent.com/78514873/199084119-a584d005-e0d7-43e3-9f67-3f7c458a0963.png">

<br>
**Significance: Searching for just "men" is important because I would like to see what article is talking about men and not the governMENt. The output lists lines that strictly has "men" as a string on its own from all txt files from all directories that are in the current directory.**
<br>
Example 2: Searching for "legal" and not include "illegal" lines.
<br>
Command: grep -w "legal" */*.txt
<br>
**Output:**
<br>
<img width="922" alt="Screen Shot 2022-10-31 at 11 42 35 AM" src="https://user-images.githubusercontent.com/78514873/199085233-0f069c24-c863-4492-b2e6-e7850a5679cf.png">

<br>
**Significance: The above example is important because I would like to view lines that only contain "legal" and not "illegal". Maybe I would like to see the context of how many times "illegal" is used vs. "not legal". The output lists all lines that have instances of legal as its own string from all txt files that are in all directories of the current directory.**
<br>
Example 3: Searching for med
<br>
Command: grep -w "med" */*.txt
<br>
**Output:**
<br>
<img width="1019" alt="Screen Shot 2022-10-31 at 11 58 03 AM" src="https://user-images.githubusercontent.com/78514873/199088066-bf09ddbf-3632-48ca-af23-45a0ea51c5ab.png">

<br>
**Significance: I wanted to search for med instead of medicine to see if authors use shortened terms. The output lists all lines that contain the string "med" and not as a substring. These lines are from all txt files that are in any directory of the current directory.**
<br>
### Method 2: Getting the line number of the string found and to read lines before/after.
<br>
#### Get the line number using: grep -n "Some String" <file1> ... <filen>
<br>
Example 1: The following is how to get the line numbers of how to get the line number of the string found from a file(s).
<br>
Command: grep -n "pregnant" */*.txt
<br>
**Output:**
<br>
<img width="834" alt="Screen Shot 2022-10-31 at 10 59 47 AM" src="https://user-images.githubusercontent.com/78514873/199078806-2cb7839c-6eb7-44af-8877-244568db54da.png">

<br>
**Significance: Knowing the line numbers of where the text is found is important because it will give the user a sense of where exactly it is located in a file and also helps with additional options such as -A and -B. which prints out lines before and after the target. The output above list not only where pregnant is found in any txt file of any directory in the current directory, it also provides which line number it is from from that file.**
<br>
#### Get the line number and (#) of text before using: grep -n -B # "Some String" <file1> ... <filen>
<br>
Example 2: The following shows how to get the line number and (# of line being 2 in this case) text before where the target string is found.
<br>
Command: grep -n -B 2 "pregnant" */*.txt
<br>
**Output:**
<br>
<img width="948" alt="Screen Shot 2022-10-31 at 11 18 10 AM" src="https://user-images.githubusercontent.com/78514873/199080845-27f1367d-b3f5-4bf1-99e8-f596e2aff458.png">

<br>
**Significance: Knowing the lines before the target word can help with the users understanding of how a word is being used. In the example above, I wanted to search for pregnant in the context of a woman who is carrying a baby. The output also provides 2 lines before the line that contains "pregnant". We find out the above example uses it as a figure of speech.**
<br>
#### Get the line number and (#) of text after using: grep -n -A # "Some String" <file1> ... <filen>
<br>
Example 3: The following shows how to get the line number and (# of line being 2 in this case) text after where the target string is found.
<br>
Command: grep -n -A 2 "pregnant" */*.txt
<br>
**Output:**
<br>
<img width="1109" alt="Screen Shot 2022-10-31 at 11 28 39 AM" src="https://user-images.githubusercontent.com/78514873/199082724-2dd326a0-c852-42ab-a92f-1a9172baf925.png">
<br>
**Significance: This example provides further context for the user of how the word is used in the context of after the target. The output from this command provides the 2 lines after in addition to the line that contains the target string "pregnant".**  
<br>
### Method 3: Get rid of case sensitivity.
<br>
#### Get rid of case sensitivity: grep -i "Some String" <file1> ... <filen>
<br>
Example 1: Searching for "alien" as its own word with -w flag.
<br>
Command: grep -wi "alien" */*.txt 
<br>
**Output:**
<br>
<img width="1129" alt="Screen Shot 2022-10-31 at 11 47 25 AM" src="https://user-images.githubusercontent.com/78514873/199086116-401a5851-609b-438d-89ed-5fe09e39829f.png">

<br>
**Significance: This example is important because it demonstrates how to find alien as its own word without case sensitivity. (Searches for Alien, alien, AlIeN, etc....). In addition, it also uses the -w flag in order to find lines that contain alien as its own string and not as a substring.**  
<br>
Example 2: Search for "trial"
<br>
Command: grep -wi "trial" */*.txt
<br>
**Output:**
<br>
<img width="1136" alt="Screen Shot 2022-10-31 at 11 51 58 AM" src="https://user-images.githubusercontent.com/78514873/199086905-519fa0ad-129e-45c2-96e3-d2e7ad8e8051.png">

<br>
**Significance: I wanted to search for all "trial"s that are not substrings in order to see each case in the different directories. The output of this command list all lines that have "trial" without case sensitivity and as a string of its own. These lines come from any txt that are from any of the directories in the current directory.**
<br>
Example 3: Searching for bomb as its own word and as a substring (without case sensitivity)
<br>
Command: grep -i "bomb" */*.txt
<br>
**Output:**
<br>
<img width="1137" alt="Screen Shot 2022-10-31 at 11 54 14 AM" src="https://user-images.githubusercontent.com/78514873/199087388-09e2b9f5-4439-4a43-b371-61a9e9ef5e39.png">

<br>
**Significance: It is also may be important for a user to see how many times a word is used as a string/substring without it being case sensitive. The output lists any line that contains the string "bomb" without case sensitivity. These lines are from any txt file that are from any directory in the current directory.**
<br>
