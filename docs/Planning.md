# Planning Stage

![Rough draft of the GUI]()

QuizController class:

Types of Questions:

- Matching: maybe with cards?
    - 4 real questions match right answer with question?
        - Only short answer question ones
    - Sure y not definitely won't be weird and unnecessary at all
- Multiple choice
    - Easiest one, just use the 4 options given
    - Vertical ABCD option under question
- Short Answer
    - SELECT all in short answer column if `short_answer = 1`
    - TextField blah blah blah
- True or false
    - Question format: Write question + ": "+answer
        - True or false radio button

General Logic:

1. Use Google Forms for "inspiration"
2. Assign type of question id's
3. Then, random num generator to pick question type
4. Select all ids for valid questions of that question type
5. Put in array and randomly select index of array
6. Call that id from table of questions
7. Repeat 5 times for each question
