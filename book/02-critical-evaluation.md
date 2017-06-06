## 2       Critical evaluation

The project could be improved in the following ways.

### 2.1     Alternative strategy for processing question and answer data

The additional functionality (to allow for any number of questions or answers) obfuscates some of the code and uses additional data structures in a clunky way (e.g. `Stack` in `FileHandler.readFile()` method).

This could have been avoided if question and answer data was handled in a more sophisticated way. This could include:
* Use of an `List` or `ArrayList`.
    * These dynamic data structures may be better able to cope with varying data sizes.
    * These was beyond the scope of the course and I am not sure exactly how to implement these.
* Use of additional classes / objects (e.g. `Question` or `WrongAnswer` class)
    * This could allow more clarity, by making data structure a part of the object oriented structure.

### 2.2     User interface

The Java Swing interface lacks elegance and gives little scope to adjust design (layout, colours, etc…)

An alternative approach could be to use a markup language e.g. HTML and CSS to allow for a more precise design.

### 2.3     Refactoring longer methods

Some methods are quite long, and could benefit from refactoring or splitting into separate methods.

Some of the worst offenders are:
* `QuizMaster.askQuestion()`
* `QuizMaster.resetQuizForSkippedQuestions()`
