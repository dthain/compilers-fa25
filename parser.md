---
layout: default
title: Parser Assignment
---

## Parser Assignment

## Objectives

The objectives of this assignment are:
- To design a grammar for a non-trivial language.
- To solve grammar ambiguities through re-writing.
- To learn how to use Bison and Flex together.
- To gain experience in incremental software engineering.

Review the [general instructions](general) for assignments.

## Overview

The next step in building a compiler is to construct a parser.
You will build upon the code from previous assignments and
use the [Bison Parser Generator](http://www.gnu.org/software/bison/manual)
to create a parser for [B-Minor Language](bminor).
It is up to you to carefully read this document and decide what all of the
relevant elements of B-Minor are.  Make sure that you include declarations,
definitions, statements, expressions, and any other program elements.

## Requirements

If your program is invoked like this:
```
./bminor --parse sourcefile.bminor
```

Then it should behave as follows:
-  If the input does not scan correctly, then `bminor` must emit `scan error:` followed by a reasonable error message and exit with status 1.
-  If the input does not parse correctly, then `bminor` must emit `parse error:` followed by a reasonable error message and exit with status 1.
-  If the input has valid B-minor syntax, then `bminor` must emit `parse successful` and exit with status 0.

If your program is invoked like this:

```
./bminor --scan sourcefile.bminor
```
Then it should continue to operate as in the previous assignment; this will facilitate debugging.
You may of course reorganize or move code around as long as the previous mode still works.

Use the scanner code from the prior assignment as your starting point.
Make sure to update your scanner to reflect the latest [standards committee decisions](https://dthain.github.io/compilers-fa25/bminor#standards-committee-clarifications).
And if your scanner has any other problems, then you should fix them before proceeding.

Make sure that the action of each scanner rule is to return a symbolic token type (e.g. `TOKEN_INTEGER_LITERAL`)
so that `yylex()` has the proper return value to be used by `yyparse()`.
You can and should fix anything in your scanner
needed to get the entire scanner-parser combination working correctly.

## General Approach

We recommend that you construct your grammar in stages and begin
by testing it on small examples, then proceeding to larger structures.
For example, start off by creating just arithmetic expressions, like this:

```
expr : expr TOKEN_ADD expr
     | expr TOKEN_SUB expr
     ...
     ;
```

Then, verify that your grammar has no shift-reduce or reduce-reduce
conflicts. If it does, look at the detailed output of Bison and re-write
your grammar rules to address them.  Once you have basic expressions working,
then start adding control-flow structures, and then declarations, until you
have constructed the complete grammar.

Note that Bison will tell you if your grammar has errors.
In particular, your grammar **must not have any shift-reduce or reduce-reduce conflicts**.  To eliminate them, you may **only re-write the production rules**, you may not apply disambiguating rules, operator precedence specifiers, or apply other "tricks" found in Bison.  (The purpose of this rule is to force you to fully understand the key ideas in LR parsing.)

It will take some time to think through the grammar problems.
Plan to work on this project over the course of several days,
so that you are able to work, then take a break to think, and
then return to the code with fresh thoughts.

## Testing

As with the previous step, create ten good test cases named `test/parser/good[0-10].bminor`
that consist of valid B-minor programs and ten bad test cases `test/parser/bad[0-10].bminor`
that scan correctly but contain parse errors.  Take the time to write thorough tests distinct from the scanner tests.

We will also evaluate your code using some hidden test cases based on the B-Minor specification.

As always, exercise good style in programming by choosing sensible
variable names, breaking complex tasks down into smaller functions,
and using constructive comments where appropriate.

Ensure that `make clean`, `make`, and `make test`, and continue to work properly.

## Development Log

For each stage of the compiler, add a new section to `devel.md` with a few thoughts on building this stage:
- What AI tools (if any) did you use, and what sort of prompts did you provide?
- What parts of the code were easy to get right?
- What parts were difficult to get right and required more effort?

## Grading

To turn in via github, please review the [general instructions for turning in](general).   Make sure that your code is tagged as a release named `parser`.

For this assignment, your grade will be based upon the following:
-  (20 points) General correctness of the code.
-  (30 points) Correctness of the grammar, including elimination of shift-reduce and reduce-reduce conflicts by the re-writing of production rules.
-  (20 points) Correctness of your submitted test cases.
-  (20 points) Correctness on the instructors' hidden test cases.
-  (10 points) Good programming style.  Each of the program components (main, scanner, parser) should be cleanly separated into multiple source files, complex or repetitive tasks should be broken into multiple functions, identifiers should be sensibly chosen, and the code generally commented and readable.

This assignment is due on **Friday, October 10th at 9:30AM**.
