## 3.       Test plan

|    |Test       |Method         |Expected Result        |Result          |Evidence       |
|-------|-----------|---------------|-----------------------|-----------------------|---------------|
|1    |"Easy" button returns easy questions  |Click on "Easy" in home screen         |Q1 is "What is cabin fever?"        |As expected          |[Screenshot](Assets/Test1.PNG)       |
|2    |"Hard" button returns hard questions  |Click on "Hard" in home screen         |Q1 is "Who likes cheese the most?"        |As expected          |[Screenshot](Assets/Test2.PNG)         |
|3    |"Quit" buttons exits gracefully       |Click "Quit" in home screen   |"Thanks for playing" dialogue displayed        |As expected          |[Screenshot](Assets/test3.PNG)         |
|4    |"OK" submits answer when question selected  |Choose all correct answers         |100% final score        |As expected          |[Screenshot](Assets/test4.PNG)        |
|5    |User prompted if "OK" clicked and no answer selected |Click "OK" without answer selected         |Dialogue prompt appears       |As expected          |[Screenshot](Assets/test5.PNG)        |
|6    |"Restart" button returns to home screen       |Click on "Restart" button         |Home screen dialogue appears        |As expected          |None       |
|7    |"Skip" button saves skipped questions until the end of the quiz       |Skip Q1 only         |Q1 appears end of quiz as "Skipped Question 1/1"        |As expected          |[Screenshot](Assets/test7_8.PNG)         |
|8    |"Skipping" for skipped questions at end of quiz       |Skip Q1 and review at end of quiz         |No "Skip" button in UI        |As expected          |[Screenshot](Assets/test7_8.PNG)         |
|9   |Correct calculates final score      |Answer all questions incorrectly         |Final Score 0% and all questions in mistake report        |As expected          |[Screenshot](Assets/test9_11.PNG)        |
|10   |Correct calculates final score      |Answer all questions correctly         |Final Score 100%        |As expected          |[Screenshot](Assets/test10.PNG)         |
|11   |Mistake report generates for all incorrect answers       |Answer all questions incorrectly and check report         |All questions in the report        |As expected          |[Screenshot](Assets/test9_11.PNG)         |
|12   |Pressing OK at end of test goes back to the home screen       |Press "OK" in final report screen         |Returns to home screen        |As expected          |None       |
|13   |Radio buttons for answers are in a random order       |Run the test twice and compare Q1 answer order         |Answers are in a different order        |As expected          |[Screenshot](Assets/test13.PNG)         |
