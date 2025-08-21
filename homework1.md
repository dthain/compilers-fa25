---
layout: default
title: Homework 1 - Compiler Stages
---

# Homework 1 - Compiler Stages

This homework should be prepared as a typed document and submitted to Canvas as a PDF.

Select a C or C++ program of your own
creation from a prior class.  It doesn't have to be very large,
but should consist of several different source files that make up a complete program.
Determine how to invoke the
different parts of the compiler (`gcc` or `g++`) in order
to create the various stages of the compiler pipeline.

Then, answer the following questions:
1. Briefly summarize the original purpose and structure of your program.
2. Count the number of files, lines, and bytes present in the source code.
3. Run the preprocessor on each source file, count the number of lines and bytes, and compare to the source files.  Examine the preprocessed code, and pick out three different fragments that are surprising to you.  Explain what's going on.
4. Run the compiler on each source file to generate object code, and again count and compare the number of bytes.  Use `nm` to observe all of the symbols in the file.  How many symbols are defined, and how many undefined?  Identify at least three undefined symbols, and look up their purpose using `man` or other reference materials, and briefly explain how they got there.
5. Generate the final executable, and again count and compare the number of bytes.  Use `nm` to observe all of the symbols in the file.  Again, count the defined and undefined symbols.  Use `ldd` to observe what dynamic libraries the program requires.  Look up the purpose of each library and briefly explain it.
6. Generate the final executable again, using the `-static` option to produce a fully statically linked executable.  Again, count the defined and undefined symbols.
7. Select one non-trivial function or method from that program, and show the complete body of that function in each stage of the compiler:
   - Original source of the function.
   - Source code after preprocessing.
   - Object code after compiling. (Use `objdump` to show readable assembly language.)
   - Executable code after linking. (Again, use `objdump`)
Comment on the evolution of the function through each of these stages.
Without knowing X86 assembly language in detail, can you identify parts
of the source code present in the assembly language output?
Is anything surprising?

Compile (ha) your answers together into one large document, taking care
to organize and format answers and code, so that it is easy to follow.
Submit one PDF document via Canvas.

**This assignment is due on Friday, August 29th.  Submit a PDF via Canvas.**

