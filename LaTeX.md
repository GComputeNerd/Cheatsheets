# LaTeX Cheatsheet

## Table of Contents

|Section|Description|
|-------|-----------|
|[Formatting](#Formatting)|A reference for Formatting|
|[Structure](#Structure)|A reference for Document Structure|
|[Text](#Text)|A reference for Text|
|[Images](#Images)|A reference for Images|
|[Tables](#Tables)|A reference for Tables|
|[Lists](#Lists)|A reference for Lists|
|[Math](#Math)|A reference for Math|
|[Bibliography](#Bibliography)|A reference for Bibliographies|
|[Packages](#Packages)|A list of Packages|
|[Environments](#Environments)|A list of Environments|
|[References](#References)|A list of LaTeX References|

## Formatting

### Table of Document Classes

|Class Name|Usage|
|----------|-----|
|article|A basic class for articles in LaTeX.|
|standalone|A class that allows TeX code to compile standalone.|

## Structure
TODO

## Text
TODO

## Images

*using graphicsx*

\graphicspath{{./images1/}{./images2/}...} Sets folders containing images.

\includegraphics{filename} Includes graphics.

|Option|Description|
|------|-----------|
|scale|Scales image by number|
|width|Sets width|
|height|Sets height|
|angle|Rotates by angle|

For positioning wrap the above command in an environment like *figure*, or *wrapfigure*

## Tables
TODO

## Lists
TODO

## Math

### Inside an amsmath environment

\tag{&lt;text&gt;} Adds &lt;text&gt; to the end of the line

### For spacing

|Command|Usage|
|-------|-----|
|\quad|18mu|
|\,|3mu|
|\:|4mu|
|\;|5mu|
|\!|-3mu|
|\ |space in normal text|
|\qquad|36mu|

## Bibliography

*Using biblatex*

\addbibresource{file.bib} imports bibliography file.

\cite{label} Adds a citation.

\printbibliography Prints full list of cited resources

### Bibliography File

File is collection of entries of the following format.

@entrytype{label,  
&nbsp;&nbsp;&nbsp;&nbsp;key=value,  
&nbsp;&nbsp;&nbsp;&nbsp;...}

entrytype can be anything from {article, book, online, manual, misc, reference, report, custom}


## Packages

|Package Name|Usage|
|------------|-----|
|asmmath|For math formatting|
|biblatex|For bibliographies|
|graphicsx|For graphics|

## Environments

### Float Environments

|Environment Name|Usage|
|----------------|-----|
|figure|Inserts a figure|
|tabular|Inserts a table|

### List Environments

|Environment Name|Usage|
|----------------|-----|
|enumerate|Ordered list|
|itemize|Unordered list|

### Math Environments

|Environment Name|Usage|
|----------------|-----|
|math|Math in paragraph mode|
|displaymath|Math in math mode|
|equation|For a single equation|
|multline|Environment breaks down long expressions and aligns it. Breaks via \\\\ |
|align|Environment aligns multiple equations, by adding an & before the = sign.|
|split|Environment can only be used inside another environment. It splits the equation and aligns, like `align` but fits the whole construct into 1 unit.|
|gather|Aligns multiple equations as groups of equations.|

## References

- https://latex.wikia.org/wiki/List_of_LaTeX_environments
- https://www.overleaf.com/learn/latex/Spacing_in_math_mode
- https://www.overleaf.com/learn/latex/Lengths_in_LaTeX
- https://www.overleaf.com/learn/latex/Aligning_equations_with_amsmath
- https://www.overleaf.com/learn/latex/Bibliography_management_with_biblatex
- https://www.overleaf.com/learn/latex/Inserting_Images
- https://ctan.org/topic/class
