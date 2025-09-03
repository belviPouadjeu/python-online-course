# Django Models Specification

## Question Model

A `Question` model will save the questions of an exam with the following characteristics:

* Used to persist questions for a course
* Has a Many-To-One relationship with the course
* Has question text
* Has a grade point for each question

## Choice Model

A `Choice` model saves all of the choices of a question:

* Many-To-One relationship with `Question` model
* The choice text
* Indicates if this choice is the correct one or not

## Submission Model

You are provided with commented out `Submission` model, which has:

* Many-to-One relationships with Exam Submissions, for example, multiple exam submissions could belong to one course enrollment.
* Many-to-Many relationship with choices or questions. For simplicity, you could relate the submission with the Choice model

You need to uncomment the `Submission` model and use it to associate selected choices.










**ER Diagram**
For your reference, we have prepared the ER diagram design for the new assesement feature.

![Onlinecourse ER Diagram](https://github.com/ibm-developer-skills-network/final-cloud-app-with-database/blob/master/static/media/course_images/onlinecourse_app_er.png)
