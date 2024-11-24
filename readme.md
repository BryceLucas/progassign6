Problem Statement
This is a 5 question website based application designed to test a users knowledge of web development technology. Including HTML, CSS, PHP, SQL, and XML. The quiz has 5 multiple choice questions each with a 15 second timer. After a question is answered the user will get feedback on if it was wrong or correct and what answer was the correct answer if they got it wrong. At the end of the quiz your score and the ability to retake or exit the quiz are available.

Functional features
- Start quiz button to initiate the quiz
- Instruction box that displays information of quiz rules before starting
- Timed questions where each question has a limit of 15 seconds
- Multiple choice questions where you can pick 1 of 4 answers
- Feedback after answers show if you are correct or if wrong shows the correct answer
- Score tracking at the end of the quiz showing your score out of 5
- progress tracker showing the current question you are on out of 5
- Result summary at the end of the quiz giving the option to retry or quit the quiz. 

Directory structure
- index.html holds the main html file that structures the content and elements of the app. 
- css folder contains the style.css file
- js folder contanins the questions.js and quizapp.js files respectively. 
In terms of file linking the <link> tag connects style.css for styling. 
the <script> tags include question.js and quizapp.js with the defer attribute to make scrips execute after html parsing.

Explanation of the code base
Index.html
- This file serves as the main structure of the quiz website.
Key sections of index.html 
- start button
- info box
- quiz box
- result box

Style.css
Defines the visual styling of the application 
- Global styles
- layout uses flexbox and positioning to center elements
- styles for all buttons
- Styling for containers, headers, timers, and the option list. 

Question.js 
Contains the data structure for the quiz questions. 
- numb question number 
- question has the text of the question
- answer has the correct answer text
- options an array of possible answer choices

quizApp.js
This file implements the logic of the quiz. 
Functions
- Showquestions(index) Displays the current question and its options
- otpionSelected(answer): Processes the users selected answer and updates the score
- startTimer(time) Initiates the countdown timer for each question
- showResult() Displays the result box when the users final question is answered. 
queCounter(index) Updates the question counter display at the bottom of the quiz box. 