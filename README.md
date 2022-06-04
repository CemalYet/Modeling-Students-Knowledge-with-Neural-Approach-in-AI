# Modeling-Students-Knowledge-with-Neural-Approach-in-AI

## Abstract
KU Leuven Massive Open Online Course (MOOC) platform provides preliminary mathematics
courses to prepare students for undergraduate programs. Students’ diverse educational back-
grounds make difficult to design a curriculum that is appropriate for all students. Knowledge Tracing
(KT) and Knowledge Space Theory (KST) are the most preferred Artificial Intelligence methods in
MOOC platforms for modeling student knowledge and providing an individual learning path to stu-
dents. Students are individually guided to achieve the desired knowledge state during training. On
the one hand, these approaches enable students to discover what they already know and should
learn to master this course. On the other hand, instructors can decide skills’ importance with a skill
relation graph provided by models. Besides, instructors can utilize models’ results to decide the
required number of questions in a pre-assessment step.

In the master’s thesis, we start by describing and comparing the KST and KT methods. Afterward,
we will examine Deep Knowledge Tracing (DKT) model, a pioneer algorithm that utilizes Long
Short Term Memory Networks (LSTM) to model student learning and predict the students’ potential
responses. At this stage, we will discuss the input expectation of DKT and, will refer to performed
data cleaning and processing steps. Meanwhile, we will highlight the limitations of our datasets and
explain their key features. Regarding implementation, we will pick hyperparameters and train the
DKT model using benchmark and KU Leuven MOOC datasets. Subsequently, we will compare our
model results with previous works. After that, we will discuss skill relation graphs obtained by DKT
models. In the meantime, we will select an appropriate question number for an assessment step
to determine students’ initial knowledge. Lastly, based on the skill relation graphs, we will advise
students on which topic they should begin the course with.

Keywords: Artificial Intelligence, Artificial Neural Networks, Deep Knowledge Tracing, Recurrent
Neural Networks, Modeling Student Knowledge.

## Requirements

You'll need Python 3.7 x64 and Tensorflow 2.0 to be able to run this project.

If you do not have Python installed yet, it is recommended that you install the [Anaconda](https://www.anaconda.com/download/) distribution of Python, which has almost all packages required in this project. You can also install Python 3.7 x64 from [here](https://www.python.org/downloads/).

Tensorflow 2.0 is installed along with the project. Check the instructions below.

## Custom Datasets

To use a different dataset, you must be sure that you have the following columns:

- **user_id**: The identifier of the student.
- **skill_id**: The identifier of the skill of the question.
- **correct**: The answer to the question [0, 1].

## Explanation
Used DKT model is taken from [lccasagrande](https://github.com/lccasagrande/Deep-Knowledge-Tracing). 
