# LaTeX report layout for university

This is a layout for a university report containing the basic building blocks I usually use in LaTeX documents.
If you want to use this layout, there are some files you have to change.

## Files to modify

1. `uni_vars.tex`: Here are some variables defined which are used in the document as placeholders (title, author, date, etc.)
2. `uni_footer.tex`: Contains the footer of the document. If you want to include a link to your university just change the example
3. `uni_main.tex`: Here you can add your chapters, sections, etc via includes.
4. `uni_preamble.tex`: add additional packages or remove some you don't need.

## Necessary programs

To build the document I added a *Makefile* which calls `pdflatex`. You should have a distribution of **LaTeX** and
also **make** installed to make use of the *Makefile*. I use **MiKTeX** for `pdflatex` and **GnuWin32** for `make`
on my Windows machine.

## Build the document

Just navigate to the root folder of this layout and run:

```bash
make
```

The generated document will be saved in `./output/uni_main.pdf`.
