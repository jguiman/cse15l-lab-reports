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
### Solution: :set number<Enter>:12,26s/start/base/g<Enter>:w<Enter>
<br>

<br>
#### Step 1: use the :set number <Enter> command in vim while in normal mode to get the line numbers of the file. This is important to know the replacement range.  
<br>
<img width="100" alt="Screen Shot 2022-11-11 at 9 42 19 PM" src="https://user-images.githubusercontent.com/78514873/201459356-1a1e72f3-bc2a-484c-9250-d366f4ecff4c.png">
<br>
#### Step 2: You will see the line range for this function block is 12 through 26. Use the command :12,26s/start base/g <Enter> while in normal mode.
<br>
### Before the command :12,26s/start/base/g<Enter> in Normal Mode.
<br>
<img width="703" alt="Screen Shot 2022-11-11 at 10 03 37 PM" src="https://user-images.githubusercontent.com/78514873/201460206-190d033e-ef63-4e92-8574-926407a5cbf3.png">
<br>
### After the command :12,26s/start/base/g<Enter> in Normal Mode. Notice it gives feedback on the bottom left of the screen and it also changed all instances of start to base in the line range from 12 to 26.
<br>
<img width="590" alt="Screen Shot 2022-11-11 at 10 12 40 PM" src="https://user-images.githubusercontent.com/78514873/201460289-30709b21-26b8-4435-bc1b-f79bf383120b.png">

<br>
#### Step 3: Enter the command :w (while in normal mode) in order to save the changes.
<br>
<img width="601" alt="Screen Shot 2022-11-11 at 10 17 07 PM" src="https://user-images.githubusercontent.com/78514873/201460455-34eb073e-4a06-4aed-8115-be8597390f13.png">

<br>
## Part 2
