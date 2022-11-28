# Lab Report #5 
<br>
## grade.sh
<br>
<img width="958" alt="Screen Shot 2022-11-28 at 11 33 59 AM" src="https://user-images.githubusercontent.com/78514873/204365102-d8891a83-2cdf-47a1-a35b-55b3f0c0c924.png">

<br>
## Student Submissions (3)
<br>
### Example 1: https://github.com/ragalina/list-examples-grader
<br>
<img width="789" alt="Screen Shot 2022-11-28 at 11 39 39 AM" src="https://user-images.githubusercontent.com/78514873/204366208-e5936894-aa97-4c01-aab2-89994a453ae7.png">
<br>
### Example 2: https://github.com/ssgadient/list-examples-grader
<br>
<img width="787" alt="Screen Shot 2022-11-28 at 11 42 45 AM" src="https://user-images.githubusercontent.com/78514873/204366735-c9da5c4d-6101-4e15-9ffc-1e68eb6d2a9a.png">

<br>
### Example 3: https://github.com/edykim/list-examples-grader
<br>
<img width="768" alt="Screen Shot 2022-11-28 at 11 44 57 AM" src="https://user-images.githubusercontent.com/78514873/204366982-981f99d4-5fc3-411b-9067-e5f7df1137d8.png">

<br>
## Trace of the Script (On Example #3)
<br>
1. rm -rf student-submission, removes student-submission folder with exit code of 0.
2. rm ListExamples.java, removes java file called ListExamples.java with exit code of 0.
3. rm ListExamples.class, removes class file called ListExamples.class with exit code of 0.
4. git clone $1 student-submission, cloned student #3's repository successfully with exit code of 0.
5. grade=0, initialize their grade.
6. if [ -e "student-submission/ListExamples.java" ], if we find ListExamples.java (which we did not and returned nonzero.)
7. else echo "The ListExamples file was not found.", this statement was printed to the out because ListExamples.java was not found.
8. echo "Your grade is $grade/3.", There grade ended up being 0/3 because we could not find ListExamples.java, the most important file of the assignment.
<br>
