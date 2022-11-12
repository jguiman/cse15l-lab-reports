# Lab Report 4
<br>
## Part 1
<br>
### Problem: Change the name of "start" parameter and all of its uses to "base"
<br>
<br>
<img width="587" alt="Screen Shot 2022-11-11 at 9 26 42 PM" src="https://user-images.githubusercontent.com/78514873/201458891-2fd37cb5-33b4-4c6d-9998-23a6d0e7dbe9.png">
<br>
#### Description: We can see, underlined in red, 3 instances of "start" being used in this block of code and want to replace it with "base".
<br>
### Solution: :set number\<Enter\>:12,26s/start/base/g\<Enter\>:w\<Enter\>
<br>

<br>
#### Step 1: use the :set number\<Enter\> command in vim while in normal mode to get the line numbers of the file. This is important to know the replacement range.  
<br>
<img width="100" alt="Screen Shot 2022-11-11 at 9 42 19 PM" src="https://user-images.githubusercontent.com/78514873/201459356-1a1e72f3-bc2a-484c-9250-d366f4ecff4c.png">
<br>
#### Step 2: You will see the line range for this function block is 12 through 26. Use the command :12,26s/start/base/g\<Enter\> while in normal mode.
<br>
### Before the command :12,26s/start/base/g\<Enter\> in Normal Mode.
<br>
<img width="703" alt="Screen Shot 2022-11-11 at 10 03 37 PM" src="https://user-images.githubusercontent.com/78514873/201460206-190d033e-ef63-4e92-8574-926407a5cbf3.png">
<br>
### After the command :12,26s/start/base/g\<Enter\> in Normal Mode. Notice it gives feedback on the bottom left of the screen and it also changed all instances of start to base in the line range from 12 to 26.
<br>
<img width="590" alt="Screen Shot 2022-11-11 at 10 12 40 PM" src="https://user-images.githubusercontent.com/78514873/201460289-30709b21-26b8-4435-bc1b-f79bf383120b.png">

<br>
#### Step 3: Enter the command :w\<Enter\> (while in normal mode) in order to save the changes.
<br>
<img width="601" alt="Screen Shot 2022-11-11 at 10 17 07 PM" src="https://user-images.githubusercontent.com/78514873/201460455-34eb073e-4a06-4aed-8115-be8597390f13.png">

<br>
<br>
## Part 2
<br>
### Two Styles of the Editing Task
<br>
#### Style 1: Start with the program opened in VisualStudioCode, make the edits there, secure copy the directory to a remote server, run bash test.sh to make sure it works.
<br>
Steps:
<br>
1. I opened visual studio code.
2. I used \<control\>+f command to show all instances of the string start.
3. I saw there were 3 instances of start in the function block.
4. For each instance, I highlighted the start with my cursor then manually typed base.
5. I moved my cursor to the top left of the screen and clicked file then save.
6. I opened a terminal from visual studio code and secure copied it to the remote server.
7. I then ssh into the server.
8. Lastly I run bash test.sh which works.
9. Overall: It was a little tedious having to manually highlight and retype start with base. It was also annoying to secure copy the directory then ssh in order to run test.sh to see if it works.
#### Style 2:
<br>
Steps:
<br>
1. I ssh into the remote server and start there.
2. I cd into docSearch and open docSearcherServer.java in vim.
3. I use the command :set number\<Enter\> to set the line numbers.
4. I use the command :12,26s/start/base/g\<Enter\> to replace the appropriate start instances with base.
5. I save and quit using the command :wq\<Enter\>
6. I run bash test.sh which works.
7. Overall: This took less steps and time compared to the first. Starting from the ssh session and the vim command made the replacements very fast and convenient. 
<br>
### Questions & Answers:
<br>
#### Q: Which of these two styles would you prefer using if you had to work on a program that you were running remotely, and why?
<br>
#### A: I would chose style 2 because it was convenient to start in the ssh session already, use the vim commands to complete the task fast, and there was less steps and overall time wasted in not having to secure copy then ssh into the remote server.
<br>
#### Q: What about the project or task might factor into your decision one way or another? (If nothing would affect your decision, say so and why!)
<br>
#### A: If I was working with a program with many files, I would use style 1 because it would be easier to navigate through different files I would have to edit. I know I can view a couple files in vim simultaneously, but it gets more difficult when there is more files to work with. However, if the project is smaller with less files I would go with style 2 because I can use the shortcuts of vim and can navigate through each file fine since there is only a few. Depending on the task, I will definitely try to use the vim shortcuts in order to save my own time. However if I don't know the vim shortcut to complete the task I want, I will have to use vscode editor to manually complete the task.
<br>
