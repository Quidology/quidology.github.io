---
layout: default
title: Planning
nav_order: 5
---

# Planning

![Rough draft of the GUI](https://quidology.github.io/assets/img/rough_sketch_gui.jpg)

## Options Explored:

### Java with JavaFX

| Pros: | Cons: |
| --- |---|
Java Desktop applications works "out-of-the-box" on many platforms | Requires a lot more storage than something over the internet
Scene Builder is convinient to build UI | Performance
CSS/FXML can seperate layout from logic | Maturity, is not that developed, less resources online

### ReactJS

| Pros: | Cons: |
| Reusable components | Lack of documentation |
| Dynamic | Requires learning a new language (JavaScript) |
|  | Web apps don't work without an Internet Connection |

### SQLite

| Pros: | Cons: |
| Affordable | Lack of documentation |
| Has all necessary functions | |
| Works without internet and well for small datasets like the quiz quesions |  |

### MySQL

| Pros: | Cons: |
| --- |---|
| Scalable | Expensive |
| High performance | Requires server to run |
|  | Needs internet to run |

## QuizController class:

### Types of Questions:

- Matching: maybe with cards?
    - 4 real questions match right answer with question?
        - Only short answer question ones
- Multiple choice
    - Easiest one, just use the 4 options given
    - Vertical ABCD option under question
- Short Answer
    - SELECT all in short answer column if `short_answer = 1`
    - TextField
- True or false
    - Question format: Write question + ": "+answer
        - True or false radio button

### General Logic:

1. Similar to online form (vertical layout)
2. Assign type of question id's
3. Then, random num generator to pick question type
4. Select all ids for valid questions of that question type
5. Put in array and randomly select index of array
6. Call that id from table of questions
7. Repeat 5 times for each question
