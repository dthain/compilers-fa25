# CSE 40243 - Compilers and Language Design - Fall 2025

MWF 9:30-10:20 in Cushing 303

## Instructors

|----|----|
|![](images/dthain-small.jpg)| Prof. Douglas Thain (`dthain@nd.edu`)<br> Office Hours: TBA <br> Office: 384 Fitpatrick Hall|

## Online Textbook

|----|----|
|![](images/compilerbook-small.jpg)| Douglas Thain,<br>Introduction to Compilers and Language Design,<br>2nd edition, 2021.<br>[http://compilerbook.org](http://compilerbook.org)

## Important Documents

- [Course Syllabus](syllabus.md)
- [Slack Channel](https://nd-cse.slack.com/channels/compilers-fa25)
- [Online Textbook](http://compilerbook.org)
- [Canvas Course Page](https://canvas.nd.edu/courses/124956)
- [Starter Code](https://github.com/dthain/compilerbook-starter-code)
- [General Assignment Instructions](general)
- [B-Minor 2025 Language Overview](bminor)

## Course Schedule

<table>

<th>
<td>
Week
<td>
Readings
<td>
Monday
<td>
Wednesday
<td>
Friday
<td>
Due Friday
<td>
Reference

<tr>
<td>
Aug 25
<td>
[Syllabus](syllabus)<br>
[Chapter 1](https://dthain.github.io/books/compiler/chapter1.pdf), [Chapter 2](https://dthain.github.io/books/compiler/chapter2.pdf)<br>
[The Absolute Minimum...](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/) 
<td>
Intro
<td>
Overview
<td>
Regular Expressions
<td>
[Homework 1](homework1)
<td>
[Regex 101](https://regex101.com/)

<tr>
<td>
Sep 1
<td>
[B-Minor 2025 Overview](bminor)<br>
[Chapter 3](https://dthain.github.io/books/compiler/chapter3.pdf)<br>
[GTA Loading Time](https://nee.lv/2021/02/28/How-I-cut-GTA-Online-loading-times-by-70/~)
<td>
RE->NFA
<td>
NFA->DFA
<td>
Flex
<td>
[Encoder Assignment](encoder)
<td>
[Hand Scanner](https://github.com/cooperative-computing-lab/cctools/blob/master/dttools/src/jx_parse.c#L254)  
[Flex Scanner Generator](https://westes.github.io/flex/manual/)

<tr>
<td>
Sep 8
<td>
[Chapter 4.1-4.2](https://dthain.github.io/books/compiler/chapter4.pdf)
<td>
CFGs
<td>
CFGs
<td>
LL(1) Grammars
<td>
Homework 2
<td>
[CFG Tool](https://web.stanford.edu/class/archive/cs/cs103/cs103.1156/tools/cfg/)
[List of Parser Generators](https://en.wikipedia.org/wiki/Comparison_of_parser_generators)

<tr>
<td>
Sep 15
<td>
[Chapter 4.2-4.3](https://dthain.github.io/books/compiler/chapter4.pdf)
<td>
LL(1) Grammars
<td>
Recursive Descent
<td>
LL(1) Table Parsing
<td>
Scanner Due
<td>

<tr>
<td>
Sep 22
<td>
[Chapter - 4.4-4.6](https://dthain.github.io/books/compiler/chapter4.pdf)
<td>
Shift-Reduce Parsing
<td>
LR(0) Automaton
<td>
SLR Parsing
<td>
Homework 3 Due


<tr>
<td>
Sep 29
<td>
[Chapter 5](https://dthain.github.io/books/compiler/chapter5.pdf)
<td>
LR(1) Parsing
<td>
Bison
<td>
Parsing B-Minor
<td>
Homework 4 Due
<td>
[Bison Manual](https://www.gnu.org/software/bison/manual/html_node/index.html)
<br>
[Bison Examples](https://github.com/dthain/compilerbook-examples/tree/master/chapter5)

<tr>
<td>
Oct 6
<td>
[Chapter 5](https://dthain.github.io/books/compiler/chapter5.pdf)
<td>
Parsing B-Minor
<td>
AST
<td>
AST
<td>
Parser Due
<td>
[AST Handout](ast.html)

<tr>
<td>
Oct 13
<td>
[Chapter 6](https://dthain.github.io/books/compiler/chapter6.pdf)
<td>
Printing
<td>
Printing
<td>
Midterm Exam
<td>

<tr>
<td>
Oct 20
<td>
[Chapter 7](https://dthain.github.io/books/compiler/chapter7.pdf)
<td>
Type Systems
<td>
Type Systems
<td>
Name Resolution
<td>
Printer Due

<tr>
<td>
Oct 27
<td>
<td>*Fall Break*
<td>*Fall Break*
<td>*Fall Break*
<td>
<td>

<tr>
<td>
Nov 3
<td>
[Chapter 7](https://dthain.github.io/books/compiler/chapter7.pdf)
<td>
<td>Checking Exprs
<td>Checking Statements
<td>Checking Decls
<td>Name Resolver Due
<td>

<tr>
<td>
Nov 10
<td>
[Chapter 9](https://dthain.github.io/books/compiler/chapter9.pdf)
<td>Memory Org
<td>Memory Org
<td>Memory Org
<td>Type Checker Due
<td>

<tr>
<td>
Nov 17
<td>
[Chapter 10](https://dthain.github.io/books/compiler/chapter10.pdf)
Ch 10
<td>Assembly
<td>Assembly
<td>Assembly
<td>
<td>[Intel Manuals](https://www.intel.com/content/www/us/en/developer/articles/technical/intel-sdm.html)
<br>
[Calling Convention](https://refspecs.linuxbase.org/elf/x86_64-abi-0.99.pdf)

<tr>
<td>
Nov 24
<td>
[Chapter 11](https://dthain.github.io/books/compiler/chapter11.pdf)
<td>Codegen
<td>*Thanksgiving*
<td>*Thanksgiving*
<td>
<td>

<tr>
<td>
Dec 1
<td>
[Chapter 11](https://dthain.github.io/books/compiler/chapter11.pdf)
<td>Codegen
<td>Codegen
<td>Codegen
<td>
<td>

<tr>
<td>
Dec 8
<td> Optimization
<td> Review<br>Codegen Due
<td> **Final Exam**<br>**7:30-9:30PM**
<td>
<td>
</table>