---
layout: default
title: Scanner Assignment
---

# Scanner Assignment

## Objectives

The objectives of this assignment are:
- To design a scanner for a non-trivial language.
- To solve identification problems with regular expressions.
- To gain experience in incremental software engineering.

## Overview 

The first step in building a compiler is to create a scanner.

You will use the [Flex Scanner Generator](https://westes.github.io/flex/manual/)
to construct a scanner generator for the [B-minor Language](bminor).
It is up to you to carefully read this document and decide what all of the
token types are, and define them carefully using Flex regular expressions.
Make sure that you define all reserved words, identifiers, operators, constants,
statements, and any other program elements.
If you think that the specification is not clear, be sure to ask for
a clarification.

Make sure that you follow the [general instructions](general) for assignments,
so that your work runs correctly on the student machines.
We want you to have the benefit of using exactly the environment in which
your work will be graded.

## Requirements

Your program will be invoked as follows:
```
./bminor --scan sourcefile.bminor
```
It must print to the standard output the
symbolic token types for each element of the input.
For literal values (integers, strings, characters) and identifiers, you
must also output the body of the token, with the quotes removed and
any escape codes translated.  If the input contains an invalid token,
then the `bminor` should print a useful message to the standard error stream
and exit with status one.  Otherwise, it should indicate success by exiting with status zero.

**Note:** Do not put `printf` statements directly into your Flex specification.
Instead, your Flex code should return the proper token type and extract the semantic
value from yytext.  (For string and character types, use the encoding functions that
you wrote in the first assignment.)  Then, let your main program call `yylex()` and
then print out the desired information.  This will make it much easier to construct the next stage.

For example, if the input looks like this:
```
while( i<10 ) { print "\'count\'", i; } @
```

Then the output should look something like this:
```
TOKEN_WHILE
TOKEN_LPAREN
TOKEN_IDENTIFIER i
TOKEN_LESSTHAN
TOKEN_INTEGER_LITERAL 10
TOKEN_RPAREN
TOKEN_LBRACE
TOKEN_PRINT
TOKEN_STRING_LITERAL 'count'
TOKEN_COMMA
TOKEN_IDENTIFIER i
TOKEN_SEMICOLON
TOKEN_RBRACE
scan error: @ is not a valid character
```

## Testing

As with the previous step, create ten good test cases named `test/scanner/good[0-10].bminor`
that consist of valid B-minor tokens and ten bad test cases `test/scanner/bad[0-10].bminor`
that contain at least one invalid token.

<strike>You can also try these [example test cases](https://github.com/dthain/compilerbook-examples/tree/master/tests/scanner) that come with the textbook but note that they don't cover the features specific to [B-Minor 2025](bminor).</strike>  Rely on your own test cases based on your reading of [B-Minor 2025](bminor).

We will evaluate your code with some additional hidden test cases for B-Minor 2025.

As always, exercise good style in programming by choosing sensible
variable names, breaking complex tasks down into smaller functions,
and using constructive comments where appropriate.

Ensure that `make clean`, `make`, and `make test`, and continue to work properly.

Update your development log to indicate what tools you used, what worked well, and what was challenging.

# Turning In

To turn in via github, please review the [General Instructions for Turning In](general).  Make sure that your code is tagged as a release named "scanner".

**This assignment is due on Thursday, September 19th at 9:30AM**

