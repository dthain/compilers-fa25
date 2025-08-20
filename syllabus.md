---
layout: default
title: Syllabus
---

# Syllabus - CSE 40243/60243 - Compilers and Language Design - Fall 2025

## Instructors

- Prof. Douglas Thain `dthain@nd.edu`
- TA: Prince Noah Johnson `pjohns24@nd.edu`

## Overview

This class will introduce you to the theory and practice of compilers,
and explore how high level language design affects the inner workings of a system.
The main goal is for you to construct a working compiler
that transforms a C-like language into X86 assembly.  This project will proceed in five
steps, requiring the construction of a scanner, parser, printer, type checker,
and code generator. Key theoretical topics will be explored through written assignments
and evaluated in exams.

This will be a fun and challenging course for advanced undergraduate students.
Compilers cover a broad array of topics in computer
science, ranging from the abstract theory of automata to the very practical details of assembly languages.
You will gain experience with tools and techniques for software engineering.
Computing this course will help you to develop a broad range of skills valuable
in the job market or graduate studies.

## Course Web Page

[http://dthain.github.io/compilers-fa25](http://dthain.github.io/compilers-fa25)

## Textbooks

- Required: [Douglas Thain, Introduction to Compilers and Language Design, 2nd edition, 2021.](http://compilerbook.org)
- Reference: Aho, Lam, Sethi, Ullman, "Compilers: Principles, Techniques, and Tools", Pearson, 2007.
- Reference: [Intel Corp, "Intel-64 and IA-32 Architectures Software Developer's Manuals", 2015](https://www.intel.com/content/www/us/en/developer/articles/technical/intel-sdm.html)

## Course Goals and Evaluation

- Discuss the role and limitations of the compiler in a computer system. (Homework 1, Midterm, Final)
- Create and analyze finite state automata for lexical analysis. (Homework 2, Scanner, Midterm)
- Create and analyze parsing algorithms for common catetgories of grammars. (Homework 3, Project 2, Midterm)
- Apply type theory to find bugs in compiled programs. (Project 3, Midterm,  Final)
- Create and analyze direct and pattern-matching code generators. (Project 4, Final)
- Understand and apply basic optimization techniques. (Final)
- Employ standard tools to create scanners, parsers, and code generators. (Projects 2, 3, and 5)
- Construct a complete working compiler for a small language. (Overall Project)

## Course Design

This course will be a mix of "low tech" and "high tech" components.
Class time and written homeworks will be organized around "low tech"
where you practice on paper and pencil to develop your mental muscles.
Programming assignments will be "high tech" and permit the use of AI
assistants for coding, building on what you learned from "low tech" skills.

### Online Textbook

First, do the assigned readings over the weekend prior to the Monday class.
Note that the textbook is dense in places; sometimes a key algorithm may only occupy
two pages in the book, but requires 30 minutes of class discussion
to work out all the details.  So, it works best if you read the textbook
slowly, taking careful notes, and then go back to review after class.

### Class Meetings

Plan to attend every meeting to the class and participate actively.
During most class sessions, I'll give a prepared lecture for about 30 minutes,
and then we will shift into Q&amp;A or working some example problems in small groups.
You should plan to take notes with pen and paper, and be ready to work problems
together on paper or on the board.

Because much of the class material involves working with data structures
and examples of algorithms, I will mostly work on the blackboard instead
of presenting slide decks.  You should take notes by sketching
along with pen and paper: the physical act of note-taking exercises your
mental muscles in a way that passive observation does not.
If you prefer to take notes on your laptop or tablet, that is acceptable.

Please refrain from using your laptops or phones
for non-class related tasks during class time.  I know it is tempting
during a brief lull to respond to messages, check the news, etc,
but even one laptop open can be an unavoidable distraction for other
people in the class.  Let's reserve this time for working together.

Note that **classes will not be recorded**, so plan accordingly.
Our class meetings are primarily for discussion and practice using the
available written materials, so if you miss class for whatever reason,
then catch up by reviewing the available materials and talking with a peer.

### Homeworks and Exams

Homework assignments will be done in a "low tech" way, and must be written
neatly **on paper by hand with a pen**, and turned in at the beginning of class
on the date due. Homeworks are an opportunity for you to practice solving problems
of the sort that you will encounter on the exams.  To that end, it is ok to work
with other students in order to get "unstuck" on a tricky problem,
as long as the end result is that you understand the material and are able to solve
problems on your own.

### Programming Assignments

The main objective of the class is for you to build a compiler from scratch,
translating the B-Minor language into X86 assembly language.  This will be
a substantial software engineering effort in which you will build the compiler
in five different stages, at each stage developing a set of thorough tests
that evaluate the correct (and incorrect) behavior of the overall tool.

Generative AI tools (e.g. ChatGPT, Gemini, Copilot, etc) are **permitted**
when working on the programming assignments.  These tools are changing quickly
and we are all still learning how to make best use of them, so consider
this a learning opportunity.  You must document any use of AI tools in the
"development log" that is part of every coding assignment.

**In any case, you remain the engineer responsible for every aspect of the code that you produce.**
My experience so far with these tools suggests that they are good at scaffolding and getting started
with a project, but tend to get confused when code reaches a certain level of complexity. 
Expect that you will need to spend substantial time thinking about and
constructing tests, troubleshooting corner cases, and understanding error messages.
This requires that you understand what the AI produces, and not just accept it blindly.

## Communications

Assignments and the course schedule are available on the course website,
and assignment grades will be posted in Canvas.
We will be using Slack (\#compilers-fa25) to handle general Q&amp;A for the class.
If you have a technical question that could be of interest to others,
please post it here, so that others can benefit from the answers.

You are welcome to post (or answer) questions anytime, and we will
generally monitor and answer questions on weekday afternoons.
(Keep in mind that we do go home at night, and so late-night questions
will get answered the next day.)

For questions about grades or anything else that just applies specifically
to you, just email the instructor or TA directly.

Office hours are a good to get focused help on a tricky bit
of code or homework problem.  We are happy to help you during that
time -- just knock, come in, and introduce yourself.
If you can't make any of the office hours, then send email to
see if we can work out another time.

## Grading Policies

All assignments must be submitted by 9:30AM on the date due (usually Fridays).
Written homeworks must be done by hand using paper and pen and turned in
at the beginning of class.  (One or two homeworks will be online PDFs instead.)
Programming assignments must be pushed to your private github repository and tagged by the same deadline.

**Late assignments will receive no credit.**  Everything in this class builds
up piece by piece, and it's important to stay on track.  If some assignment isn't
working out perfectly, it's usally best to submit what you have on time, and keep moving.

You are permitted **one free late pass* to account for the ordinary circumstances of
life, such as a minor illness, schedule conflict, etc.  To do so, just
send an email to the TA **before the deadline**, saying briefly "I would like to take a late pass on assignment X".
And the due date for that item will be extended by seven calendar days.
(Sorry, you can't use a late pass on the final assignment.)

Beyond that, exceptions will only be made for serious circumstances
such as a hospitalization, death in the family,
mandatory participation in a university sponsored event,
or the other items outlined in section 3.1 of the Undergraduate Academic Code.
In those cases, please confer with the instructor at the earliest possibility.

For each assignment, a numeric grade will be awarded.
Throughout the semester, grades and class averages will be posted through Sakai.
At the end of the semester, I'll convert number grades to letter grades on
a scale of A/B/C/D = 90/80/70/65, and exercise some prudential judgement
for pluses and minuses and borderline grades.

If you believe that an error has been made in grading an item,
please bring it to the attention of the person who graded it
(usually the TA) within seven days. Mistakes do occasionally
happen in grading, so factual and clerical errors will be
cheerfully corrected.  Matters of judgement are reserved to the TA.
If, after talking to the TA, you are unconvinced,
you can bring it up with Prof. Thain.

grades are weighted as follows:
Written Homeworks 20%, Programming Assignments 40%, Midterm 20%, Final 20%.

## Academic Code of Honor

As a student at Notre Dame, you are bound by the [Academic Code of Honor] (http://honorcode.nd.edu),
which states:

*As a member of the Notre Dame community, I acknowledge that it is my responsibility to learn and abide by principles of intellectual honesty and academic integrity, and therefore I will not participate in or tolerate academic dishonesty.*

The purpose of the homeworks and assignments in this course is for you
to gain the discipline and skills in analysis, design, and programming so that
you will be able to work independently in a professional setting.
To that end, all work in this class must be the result of your own ideas and effort.

You are permitted to consult with other students, search engines,
and AI assistants in order to find documentation, troubleshoot technical
problems, and generally get "unstuck" after making your own efforts.
However, the outcome of such consultation must
be that you understand *what it means* and *how to do it yourself*.
You remain responsible for all work that bears your name.

## Some Campus Resources

- If you require an accommodation for a disability, please first contact the
Sara Bea Center [http://sarabeadisabilityservices.nd.edu](sarabeadisabilityservices.nd.edu) for a consultation, and we will be happy to work together on a solution.
-  If you encounter a difficult life situation and don't know what to do,
the University Counseling Center [http://ucc.nd.edu](http://ucc.nd.edu) or the Care and Wellness Consultants [http://care.nd.edu](care.nd.edu) can help and also connect you with other campus resources.
