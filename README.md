# Final Project: MAP - Charting Student Math Misunderstandings

## Problem and goals 

This project aims to develop a machine learning-based natural language processing (NLP) model that can predict students’ potential math misconceptions based on their open-ended written explanations. By identifying patterns of incorrect reasoning across diverse problems, the goal is to support scalable, diagnostic feedback for teachers, ultimately improving student learning and conceptual understanding in mathematics.

## Data

- **Source:** The dataset originates from the Eedi platform, where students respond to Diagnostic Questions (DQs)—multiple-choice math questions with one correct answer and three distractors. After answering, some students provide written justifications, which form the core of the Misconception Annotation Project (MAP) dataset.

- **Structure and Dimensions:** Each row in the dataset captures a student's response to a single question, including the selected answer and their accompanying explanation. The dataset includes the following fields: QuestionId, QuestionText, MC_Answer, StudentExplanation, Category (train only), and Misconception (train only). The Category field indicates whether the multiple-choice response was correct and whether the explanation contained a misconception (e.g., True_Misconception). If a misconception is present, the Misconception field names it; otherwise, it is marked as 'NA'.

- **Size:** The re-run test data comprises approximately 16,000 student responses. The full dataset includes separate training and test CSV files, as well as a sample submission file that requires predictions in the format: Category:Misconception, allowing up to three predicted pairs per instance.

- **Download:**

https://www.kaggle.com/competitions/map-charting-student-math-misunderstandings
