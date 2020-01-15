# DHBW-PA5-Preset

A LaTeX preset for the fifth "Praxisarbeit" at the Duale Hochschule Baden-Württemberg Mannheim, quite different from the usual.

## Compiling

```sh
$ latexmk PA.tex
```

with XeLaTeX (already specified in the `.latexmkrc`). Target document is `PA.pdf`.

## Content

### Settings

You will have to fill in title, author, "Matrikelnummer", time and place you are signing, e-mail, and employer.

### Restriction

If your thesis must contain a "Sperrvermerk", you have to uncomment the line in `PA.tex`.

### Abbrevations and bibliography

Examples provided (please remove before turning in) in `inhalt/Abkuerzungen.tex` and `PA.bib`, respectively.

### Abstract

Abstract is `inhalt/Abstract.tex`.

### Main content

Some more usage examples are in `inhalt/1.tex`. You are advised to split your content into `inhalt/1.tex`, `inhalt/2.tex`, etc., and `\include` it respectively.

### Fork Changes
- Added some helpfull packages in PA.tex
- Adding document root to all "standard" .tex files
- Adding central chapter management

To compile the document from every .tex file add
```
%!TEX root = ../../PA.tex
%!BIB program = biber
```
at the top of the file. (Important: check if the path to root is right!)
