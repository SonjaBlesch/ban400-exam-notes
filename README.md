# Exam notes for the BAN400 exam

This repository contains notes that, under certain conditions, will be made available on the BAN400 exam. The document will be updated via pull requests from the students. Please read the instructions below carefully before submitting changes. Pull requests that do not follow the standards set out in this document will be rejected.

If the contributions encompass a substantial amount of the course by **1 December 2024**, the file `ban400-exam-notes.pdf` will be handed out as attachment to the exam.

## Structure of the repository

The main document in this repository is `ban400-exam-notes.pdf`, which is generated from the Quarto file `ban400-exam-notes.qmd`. This source document automatically collects content from the two folders `functions/` and `topics/` and should **not** be changed or compiled as part of a pull request. 

The note contains two main sections:

- **Functions.** This section contains tables of functions with a short description, organized by topic. 
- **Topics.** This section contains very short memos of topics and various programming structures that we have covered in the course. These snippets may contain a brief introduction (a few sentences) and some general code that shows the syntax. 

## How to contribute

All pull requests must be changes or additions to the content in the folders `functions/` or `topics/`.

### Functions

The functions listed in the first section of the document are collected from `.csv`-files in the folder `functions/`. The naming convention for these files is `XX-some_headline.csv` where `XX` is a two digit number indicating the sequence that the files will be displayed in the final document, and `some_headline` is a descriptive headline for this group of functions. 

There must be a *dash* between the sequence and the headline, and the headline must be all lowercase letters with *underscore* separating the words. 

The file itself must be comma separated with exactly three column headers:
- `function_name`: contains the name of the function. All function names must be followed by a pair of parentheses. 
- `package`: indicates which package that contains the function.
- `short_description`: contains the shortest possible description of the purpose of the function. Do not enter further information about arguments, examples of use, etc, into this field. All of that is available in the documentation of the function. 

### Topics

This folder contains short descriptions and syntax of various coding structures and concepts from the course. The topics are collected in separate `.qmd`-files that must comply with the following conventions:

- The file name is descriptive for the contents and all lowercase letters in snake case, with file type `.qmd`.
- The title in the file should be a third level headline (`###`) and descriptive for the contents. 
- One additional level of subheaders (`####`) is allowed. 
- Text should be extremely short, to-the-point, with the main purpose of introducing an example of syntax.
- All code must be set in code environment, either inline or as a code block. 
- Code blocks must be pure R-blocks with no additional options. The code is not run when compiling the document so it need not be "valid" in the sense that all variables must be defined, etc., but the code must obviously be *correct*.

## Further provisions

- A pull request should only contain changes/additions to the raw content files as described above. This means that you should *not* compile the document. This will be done after the changes have been accepted. 
- Make sure that you have pulled the latest changes to the fork before opening your pull request and that there are no conflicts. 
- In order to minimize the potential for conflicts, you should prioritize opening several smaller pull requests rather than one big.
- **The note will be considered for possible attachment to the exam questions shortly after 01 December 2025. The note does not have to be particularly long for this to happen, but there must be a reasonably large coverage of the foundations of the curriculum in BAN400.**


