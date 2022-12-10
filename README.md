# Research Report: Data Science for Healthcare
#### (Data Science at UCLan)
![GPLv2][license-badge]

#### BRIEF:

> You will choose an area of business and a specific Use Case in which data science is exploited (or has the potential) to bring competitive advantage.
> You will critically discuss the application of data science, including the:
>
> - acquisition of specific data sources,
> - data processing,
> - algorithm selection,
> - data visualisation and,
> - data analysis and methods for interpretation of results.
> Critically evaluate the case for or against adoption (or current/developing application) of data science for your chosen business and specific Use Case.

For the complete brief, click [here][brief].

The area of business chosen was the **healthcare** industry and the specific use case is the **prediction of diseases**.



## Building

##### latexmk

```bash
$ latexmk -pdf
```



##### pdflatex

```bash
$ pdflatex -shell-escape report.tex
# Build references
$ biber report
# Run again to load references
$ pdflatex -shell-escape report.tex
```



##### to Word document

```bash
# Conversion is not perfect and still requires tweaks
$ pandoc report.tex -f latex -t docx -o report.docx --bibliography=references.bib
```



## Authorship

**Jacob Sanchez Perez \<jsanchez-perez@uclan.ac.uk>**



## License

![GPLv2][license-badge]

This software is distributed under the [General Public License v2.0][license], more information available at the [Free Software Foundation][gnu].

[uclan]: https://uclan.ac.uk

[brief]: Assignment_1_Brief.docx "Assignment 1 Brief"

[license]: LICENSE "General Public License"
[gnu]: https://www.gnu.org/licenses/old-licenses/gpl-2.0.html "Free Software Foundation"

[license-badge]: https://img.shields.io/github/license/jacobszpz/DataScienceForHealthcare
