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


# Task 4: Test Data

You will now create test data for your application.

## Add Instructor

Add `admin` as an Instructor

## Course Information

| Field | Value |
|-------|-------|
| Name | Learning Django |
| Image | Download from here |
| Description | Django is an extremely popular and fully featured server-side web framework, written in Python |
| Pub date | Today |
| Instructors | admin |

### Lesson Information

| Field | Value |
|-------|-------|
| Lesson #1 Title | What is Django |
| Lesson #1 Order | 0 |
| Lesson #1 Content | Django is a high-level Python web framework that encourages rapid development and clean, pragmatic design. Built by experienced developers, it takes care of much of the hassle of web development, so you can focus on writing your app without needing to reinvent the wheel. It's free and open source. |

## Test Question

| Field | Value |
|-------|-------|
| Course | Name: Learning Django, Description: ... |
| Content | Is Django a Python framework |
| Grade | 100 |

### Choices

| Field | Value |
|-------|-------|
| Choice #1 Content | Yes |
| Choice #1 Is correct | ✓ |
| Choice #2 Content | No |
| Choice #2 Is correct | *Leave blank* |

