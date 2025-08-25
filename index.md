---
title: CSE 30341 - Compilers and Language design - Fall 2025
layout: default
---

# CSE 40243 - Compilers and Language Design - Fall 2025

MWF 9:30-10:20 in Cushing 303

## Instructors

<table markdown="0">
<tr>
<td><img src="images/dthain.jpg" height=128/></td>
<td> 
Prof. Douglas Thain (<tt>dthain@nd.edu</tt>)<br>
Office Hours: TBA<br>
Office: 384 Fitpatrick Hall
</td>
</tr>
<tr>
<td><img src="images/pjohns24.jpg" height=128/></td>
<td>
TA: Prince Noah Johnson (<tt>pjohns24@nd.edu</tt>)<br>
Office Hours: TBA<br>
Office: CSE Student Commons
</td>
</tr>
</table>

## Online Textbook

<table markdown="0">
<tr>
<td><img src="images/compilerbook-small.jpg"></td>
<td>
Douglas Thain,<br>
Introduction to Compilers and Language Design,<br>
2nd edition, 2021.<br>
<a href="http://compilerbook.org">http://compilerbook.org</a>
</td>
</tr>
</table>


## Important Documents

- [Course Syllabus](syllabus)
- [Slack Channel](https://nd-cse.slack.com/channels/compilers-fa25)
- [Online Textbook](http://compilerbook.org)
- [Canvas Course Page](https://canvas.nd.edu/courses/124956)
- [Starter Code](https://github.com/dthain/compilerbook-starter-code)
- [General Assignment Instructions](general)
- [B-Minor 2025 Language Overview](bminor)

## Course Schedule

<table markdown="0">

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
<li><a href=syllabus>Syllabus</a>
<li><a href="https://dthain.github.io/books/compiler/chapter1.pdf">Chapter 1</a>
<li><a href="https://dthain.github.io/books/compiler/chapter2.pdf">Chapter 2</a>
<li><a href="https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/">The&nbsp;Absolute&nbsp;Minimum...</a>
<td>
<a href="https://docs.google.com/presentation/d/1rjtXRK-gbc9ZA4RW97zVnwUZLxlr_mDndqCMHPiy-mo/edit">Overview</a>
<td>
Compiler Stages
<td>
Regular Expressions
<td>
<strong><a href="homework1">Homework&nbsp;1</a></strong>
<td>
<a href="https://regex101.com/">Regex 101</a>

<tr>
<td>
Sep 1
<td>
<li><a href="https://dthain.github.io/books/compiler/chapter3.pdf">Chapter 3</a><br>
<li><a href="bminor">B-Minor&nbsp;2025</a><br>
<li><a href="https://nee.lv/2021/02/28/How-I-cut-GTA-Online-loading-times-by-70/">GTA&nbsp;Loading&nbsp;Time</a>
<td>
RE->NFA
<td>
NFA->DFA
<td>
Flex
<td>
<strong><a href="encoder">Encoder Due</a></strong>
<td>
<a href="https://github.com/cooperative-computing-lab/cctools/blob/master/dttools/src/jx_parse.c#L254">Hand&nbsp;Scanner</a><br>
<a href="https://westes.github.io/flex/manual/">Flex&nbsp;Scanner&nbsp;Generator</a><br>

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
<strong>Homework 2</strong>
<td>
<a href="https://web.stanford.edu/class/archive/cs/cs103/cs103.1156/tools/cfg/">CFG&nbsp;Tool</a><br>
<a href="https://en.wikipedia.org/wiki/Comparison_of_parser_generators">Parser&nbsp;Generators</a><br>

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
<strong>Scanner Due</strong>
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
<strong>Homework 3</strong>
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
<strong>Homework 4</strong>
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
<strong>Parser Due</strong>
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
<strong>Midterm&nbsp;Exam</strong>
<td>
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
<td>

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
<td>Checking Exprs
<td>Checking Statements
<td>Checking Decls
<td><strong>Resolver Due</strong>
<td>

<tr>
<td>
Nov 10
<td>
<a href="https://dthain.github.io/books/compiler/chapter9.pdf">Chapter 9</a>
<td>Memory&nbsp;Org
<td>Memory&nbsp;Org
<td>Memory&nbsp;Org
<td><strong>Type Checker Due</strong>
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
<td>Codegen Exprs
<td><i>Thanksgiving</i>
<td><i>Thanksgiving</i>
<td>
<td>

<tr>
<td>
Dec 1
<td>
<a href="https://dthain.github.io/books/compiler/chapter12.pdf">Chapter 12</a>
<td>Codegen Stmts
<td>Codegen Decls
<td>Optimization
<td>
<td>

<tr>
<td>
Dec 8
<td>
<a href="https://dthain.github.io/books/compiler/chapter12.pdf">Chapter 12</a>
<td> Optimization
<td> Review<br><strong>Codegen Due</strong>
<td> <strong>Final Exam</strong><br><strong>7:30-9:30PM</strong>
<td>
<td>

</table>
