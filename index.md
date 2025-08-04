# CSE 40243 - Compilers and Language Design - Fall 2025

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
- [Canvas Course Page](https://canvas.nd.edu/courses/70800)
- [Starter Code](https://github.com/dthain/compilerbook-starter-code)
- [General Assignment Instructions](general)
- [B-Minor 2025 Language Overview](bminor)
- [Flex Scanner Generator](https://westes.github.io/flex/manual/)
- [Bison Parser Generator](https://www.gnu.org/software/bison/manual/html_node/index.html)

## Course Schedule

(Subject to change as needed.)

|Week | Reading      | Due Monday      | Monday        | Wednesday    |Friday       | Extra Links |
|-----|--------------|-----------------|---------------|--------------|-------------|-------------|
|Aug 25 | Ch 1-2     | Intro<br>[Syllabus](syllabus.md)| Overview     | Regular Expressions<br> **[HW1 Due](homework)**  | [Unicode](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/) <br> [Regex 101](https://regex101.com/) <br> [Regex Golf](http://alf.nu/RegexGolf?world=regex&level=r02) <br>
|Sep 1  | Ch 3       | Encoder Due     | Finite Automata | RE->NFA           | NFA->DFA                    | [Hand Scanner](https://github.com/cooperative-computing-lab/cctools/blob/master/dttools/src/jx_parse.c#L254)
|Sep 8  | Ch 3       | HW2 Due         | Flex            | CFGs              | CFGs                        | [Flex Scanner Generator](https://westes.github.io/flex/manual/)
|Sep 15 | Ch 4.1-4.3 | Scanner Due     | LL(1) Grammars  | Recursive Descent | LL(1) Table Parsing         |
|Sep 22 | Ch 4.4-4.6 | HW3 Due         | Shift-Reduce Parsing | LR(0) Automaton | SLR Parsing              |
|Sep 29 | Ch 5       |                 | LR(1) Parsing   | Bison             | Parsing B-Minor            | [Bison Examples](https://github.com/dthain/compilerbook-examples/tree/master/chapter5)
|Oct 6  | Ch 5       | HW4 Due         | Parsing B-Minor | AST               | AST                         | [AST Handout](ast.html) |
|Oct 13 | Ch 6       | Parser Due      | AST / Printing  | Review            | **[Midterm Exam](midterm)** |
|Oct 20 | Ch 7       | Printer Due     | Type Systems    | Type Systems      | Name Resolution             |
|Oct 27 |            |                 | *Fall Break*    | *Fall Break*      | *Fall Break*                |
|Nov 3  | Ch 7       |                 | Typechecking    | Typechecking      | Typechecking                |
|Nov 10 | Ch 9       | Resolver Due    | Memory Org      | Memory Org        | Memory Org                  | 
|Nov 17 | Ch 10      | Typechecker Due | Assembly        | Assembly          | Assembly                    | [Intel Manuals](https://www.intel.com/content/www/us/en/developer/articles/technical/intel-sdm.html) <br> [Calling Convention](https://refspecs.linuxbase.org/elf/x86_64-abi-0.99.pdf)
|Nov 24 | Ch 11      |                 | Codegen         | *Thanksgiving*    | *Thanksgiving*              |
|Dec 1  | Ch 11      |                 | Codegen         | Codegen           | Codegen                     |
|Dec 8  |            | Codegen Due     | Optimization    | Review            | *Exam Week*                 |
|Dec 15 |            |                 | *Exam Week*     | *Exam Week*       | *Exam Week*                 |

<!--
[CFG Tool](https://web.stanford.edu/class/archive/cs/cs103/cs103.1156/tools/cfg/)
[Joke](https://xkcd.com/1090/)
[Bison Manual](https://www.gnu.org/software/bison/manual/html_node/index.html)
[Bison Examples](https://github.com/dthain/compilerbook-examples/tree/master/chapter5)
-->
