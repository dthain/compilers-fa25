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

<tr>
<th>
Week
<th>
Readings
<th>
Monday
<th>
Wednesday
<th>
Friday
<th>
Due Friday
<th>
Reference

<tr>
<td>
Aug 25
<td>
<a href=syllabus>Syllabus</a><br>
<a href="https://dthain.github.io/books/compiler/chapter1.pdf">Chapter 1</a>, <a href="https://dthain.github.io/books/compiler/chapter2.pdf">Chapter 2</a><br>
<a href="https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/">The &nbsp;Absolute&nbsp;Minimum...</a> 
<td>
Intro
<td>
Overview
<td>
Regular Expressions
<td>
<a href="homework1">Homework 1</a>
<td>
<a href="https://regex101.com/">Regex 101</a>

<tr>
<td>
Sep 1
<td>
<a href="bminor">B-Minor&nbsp;2025</a><br>
<a href="https://dthain.github.io/books/compiler/chapter3.pdf">Chapter 3</a><br>
<a href="https://nee.lv/2021/02/28/How-I-cut-GTA-Online-loading-times-by-70/~">GTA&nbsp;Loading&nbsp;Time</a>
<td>
RE->NFA
<td>
NFA->DFA
<td>
Flex
<td>
<a href="encoder">Encoder Assignment</a>
<td>
<a href="https://github.com/cooperative-computing-lab/cctools/blob/master/dttools/src/jx_parse.c#L254">Hand Scanner</a>  
<a href="https://westes.github.io/flex/manual/">Flex Scanner Generator</a>

<tr>
<td>
Sep 8
<td>
<a href="https://dthain.github.io/books/compiler/chapter4.pdf">Chapter 4.1-4.2</a>
<td>
CFGs
<td>
CFGs
<td>
LL(1) Grammars
<td>
Homework 2
<td>
<a href="https://web.stanford.edu/class/archive/cs/cs103/cs103.1156/tools/cfg/">CFG&nbsp;Tool</a>
<a href="https://en.wikipedia.org/wiki/Comparison_of_parser_generators">Parser&nbsp;Generators</a>

<tr>
<td>
Sep 15
<td>
<a href="https://dthain.github.io/books/compiler/chapter4.pdf">Chapter 4.2-4.3</a>
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
<a href="https://dthain.github.io/books/compiler/chapter4.pdf">Chapter 4.4-4.6</a>
<td>
Shift-Reduce Parsing
<td>
LR(0) Automaton
<td>
SLR Parsing
<td>
Homework 3 Due
<td>

<tr>
<td>
Sep 29
<td>
<a href="https://dthain.github.io/books/compiler/chapter5.pdf">Chapter 5</a>
<td>
LR(1) Parsing
<td>
Bison
<td>
Parsing B-Minor
<td>
Homework 4 Due
<td>
<a href="https://www.gnu.org/software/bison/manual/html_node/index.html">Bison&nbsp;Manual</a>
<br>
<a href="https://github.com/dthain/compilerbook-examples/tree/master/chapter5">Bison&nbsp;Examples</a>

<tr>
<td>
Oct 6
<td>
<a href="https://dthain.github.io/books/compiler/chapter5.pdf">Chapter 5</a>
<td>
Parsing B-Minor
<td>
AST
<td>
AST
<td>
Parser Due
<td>
<a href="ast.html">AST Handout</a>

<tr>
<td>
Oct 13
<td>
<a href="https://dthain.github.io/books/compiler/chapter6.pdf">Chapter 6</a>
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
<a href="https://dthain.github.io/books/compiler/chapter7.pdf">Chapter 7</a>
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
<td><i>Fall&nbsp;Break</i>
<td><i>Fall&nbsp;Break</i>
<td><i>Fall&nbsp;Break</i>
<td>
<td>

<tr>
<td>
Nov 3
<td>
<a href="https://dthain.github.io/books/compiler/chapter7.pdf">Chapter 7</a>
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
<a href="https://dthain.github.io/books/compiler/chapter9.pdf">Chapter 9</a>
<td>Memory&nbsp;Org
<td>Memory&nbsp;Org
<td>Memory&nbsp;Org
<td>Type Checker Due
<td>

<tr>
<td>
Nov 17
<td>
<a href="https://dthain.github.io/books/compiler/chapter10.pdf">Chapter 10</a>
<td>Assembly
<td>Assembly
<td>Assembly
<td>
<td><a href="https://www.intel.com/content/www/us/en/developer/articles/technical/intel-sdm.html">Intel&nbsp;Manuals</a>
<br>
<a href="https://refspecs.linuxbase.org/elf/x86_64-abi-0.99.pdf">Calling&nbsp;Convention</a>

<tr>
<td>
Nov 24
<td>
<a href="https://dthain.github.io/books/compiler/chapter11.pdf">Chapter 11</a>
<td>Codegen
<td><i>Thanksgiving</i>
<td><i>Thanksgiving</i>
<td>
<td>

<tr>
<td>
Dec 1
<td>
<a href="https://dthain.github.io/books/compiler/chapter11.pdf">Chapter 11</a>
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
<td> <b>Final Exam</b><br><b>7:30-9:30PM</b>
<td>
<td>
