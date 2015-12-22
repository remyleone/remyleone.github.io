---
layout: article
title: My LaTeX Workflow to avoid spelling mistakes
teaser: Some useful tips for your LaTeX projects
categories: [code]
tags: [latex]
published: True
---

I use several tools and techniques to ensure that my Latex is as good as
possible.

## LaTeX tools

### Nag

[Nag](//www.ctan.org/tex-archive/macros/latex/contrib/nag) is a tool to help
you detect old commands and deprecated LaTeX code.

Simply put the following lines in your code:

{% highlight latex %}
\RequirePackage[l2tabu, orthodox]{nag}
{% endhighlight %}

### latexmk

[Latexmk](//users.phys.psu.edu/~collins/software/latexmk-jcc/) is a very good
tool to never have to worry anymore about how many time you have to compile to
get your bibliography right. A latemkrc is the file you will put inside the
project that will help bootstrap latexmk. Here's mine:

{% highlight perl %}
$pdf_mode = "1";
$pdflatex = "pdflatex";
$makeindex = "splitindex";
$makeindex = "makeindex;splitindex;";
{% endhighlight %}

## Spelling help

### Language tool

[Language tool](//languagetool.org) is Java grammar checker. It helps detect
grammar mistakes such as _He play tennis_ and many others. I usually launch
the checker against all my tex folder. If you use
[TeXstudio](//www.texstudio.org) you can have [Language
tool](//languagetool.org) directly integrated inside your editor:

[Checking (La)TeX With LanguageTool - LanguageTool Wiki](//wiki.languagetool.org/checking-la-tex-with-languagetool)

### Pandoc + Microsoft Office

[Pandoc](//johnmacfarlane.net/pandoc) is like a swiss-army knife for
converting text back and forth in different format.

Suppose that you have a large body of text in LaTeX and you want to convert it
to a docx format to spell check it on Microsoft Office. By using pandoc you
could have it quickly:

	pandoc main.tex -o main.docx

That's it! Now, you have a main.docx that you can pass along to other grammar
checker such as the one embedded in Microsoft Word.

## Project layout

I like to have a modular project. Therefore, I use the following layout:


	├── myproject.sublime-project
	├── myproject.sublime-workspace
	├── IEEEtran.cls
	├── latexmkrc
	├── main.pdf
	├── main.tex
	├── Makefile
	├── readme.md
	├── main.bib
	└── tex
	    ├── abstract.tex
	    ├── conclusion.tex
	    ├── experiment.tex
	    ├── intro.tex
	    └── related.tex

A main.tex document that import all other using similar snippets:

{% highlight latex %}
\begin{document}

\maketitle

\input{tex/abstract}
\input{tex/intro}
\input{tex/related}
\input{tex/experiment}
\input{tex/conclusion}

\end{document}
{% endhighlight %}

Organizing code this way is handy because I only have small files that I can
easily get on one screen, share in an email or simply read in one sight. If my
code was a monolithic file with thoushands of lines, it would be much harder
to see where I am in the structure.

Plus if you use an editor such as [Vim](//www.vim.org) (plus the
[Ctrl-p](//github.com/kien/ctrlp.vim) plugin) or [Sublime
Text](//sublimetext.com) you can open any file you want by simply typing
Ctrl-p and going in very few key strokes anywhere in your document.

### Makefile

Of course, you don't want to type commands all the time. Therefore you put
them in a makefile like this one:

{% highlight Makefile %}
all:
        latexmk

clean:
        latexmk -C
{% endhighlight %}
