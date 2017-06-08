## 1       Project overview

### 1.1	    Object Oriented Structure

To give the project a logical structure it divides functionality into 3 classes:

* `Quiz.java`
	* A higher level class that oversees the entire quiz process.
* `FileHandler.java`
	* Manages all file interaction. Get questions and answers from text files and process them into correct data structures.
* `QuizMaster.java`
	* Handles the mechanics of asking questions and accepting answers. Includes an option to skip questions. Does most of the heavy lifting of the UI, using Java Swing.

### 1.2 	Additional features

The project implements all basic and advanced requirements in the specification. It also includes some additional code to allow for:

#### 1.2.1	Any number of questions or answers

The quiz is made of 10 questions in each difficulty mode, but could accommodate:

* Any number of questions, not just 10
* Any number of possible answers, including a different number of possible answers in different questions.

These features require some additional code to process differing length data sizes into fixed length arrays. Examples of this additional code can be found in these methods:

* `FileHandler.readFile()`
    * Uses a `Stack` to check number of questions before initialising and populating a fixed length `String[]` array.
* `FileHandler.getTextAs2DArray()`
    * Requires two loops. One to check maximum length before initialising the array, and then another loop to populate the array.
* `QuizMaster.combineAnswers()`
    * Uses a `Stack` to check number of answers before initialising and populating a fixed length `String[]` array.

#### 1.2.2 Randomises answers for display
Answer options are displayed in a random order each time a question is asked. This is implemented by:

* `QuizMaster.jumbleAnswers()`