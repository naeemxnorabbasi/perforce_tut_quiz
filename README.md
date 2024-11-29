# Perforce Tutorial Compilation Guide

Files
- `Makefile`: Automates the compilation of LaTeX documents.
- `p4_tut.tex`: LaTeX source file for the Perforce Tutorial.
- `p4_quiz.tex`: LaTeX source file for the Perforce Quizzes and Answers.
- `p4_tut.pdf`: Compiled PDF of the Perforce Tutorial.
- `p4_quiz.pdf`: Compiled PDF of the Perforce Quizzes and Answers.
- `README.md`: This readme file with instructions.

# Compilation Instructions

**To compile the LaTeX documents and generate the PDFs, follow these steps:**

Ensure you have LaTeX installed on your system. You can install TeX Live or MiKTeX depending on your operating system.

Open a terminal in the directory containing the files.

**Run the Makefile by executing:**
```bash
make
```
This command will compile both p4_tut.tex and p4_quiz.tex, producing p4_tut.pdf and p4_quiz.pdf respectively.

**Clean auxiliary files (optional):**
To remove auxiliary files generated during compilation, run:
```bash
make clean
```

**Remove all generated files (including PDFs):**
To clean up all compiled files and PDFs, run:
```bash
make mrproper
```
**Notes**

The `Makefile` is configured to compile all `.tex` files listed in the TEXFILES variable.
The `pdflatex` command is run twice to ensure that all references, such as the table of contents, are updated correctly.
Ensure that all `.tex` files are in the same directory as the `Makefile` when compiling.


**Compile Using the Makefile:**

   With all the files in the same directory, you can compile the documents as instructed in the `README.md`.

**Example Terminal Commands:**

```bash
# Compile both documents
make

# Clean auxiliary files
make clean

# Remove all generated files including PDFs
make mrproper
