---
layout: lesson
title: Writing guide (aimed at writing in Dutch)
category: week2
description: Nederlandse stijlregels voor wiskunde en LaTeX.
---

In this lesson we cover some rules of thumb for writing down mathematics. The first paragraph is about writing down maths in general. The rules of thumb for this are independent of LaTeX. In the second paragraph you will learn about how to LaTeX mathematical articles or other projects.
Here is a [pdf-version of the writing guide](schrijfgids2013.pdf) in Dutch.

A. Writing down mathematics
---------------------------

Thinking up new things in maths is impressive, but it is just as important to write it down well. By paying attention to the following points you will help your text's reader immensely.

### A.1. Write sentences starting with capital letter and ending in a period

Writing a mathematical text is not any different than writing any other text in your target language. A text is made up of sentences. Every sentence starts with a capital letter and ends in a period. 

You should never start a sentence with a formula. Add some words in first:

<div class="example">
We have \$a=1\$. We see that \$f(1) = \pi\$.
</div>

The same goes for symbols:

<div class="example" markdown="0">
The number $n$ is important. The function $f$ is real. 
</div>

A sentence always ends in a period, also when the sentence ends in a formula:

<div class="example" markdown="0">
Define an integer $n \not= 0$ en definieer

\[
(\Z/n\Z)^* = \{a \in \Z/n\Z : \gcd(a, n) = 1\}.
\]
</div>

If a sentence continues after the equation, use appropriate punctiation, for example a comma:

<div class="example" markdown="0">
For $n\geq 2$, the sign defines a surjective homomorphism

\[

\varepsilon : S_n \to \{+1, -1\},

\]

which is to say, $\varepsilon(\sigma \tau) =
\varepsilon(\sigma)\varepsilon(\tau)$ for all $\sigma,\tau
\in S_n$.

</div>

### A.2. Divide the text into paragraphs and sections

Sentences which have similar or connecting content should form a paragraph. The beginning of a paragraph has an *indent* by default, which clearly marks the beginning of a new paragraph. Remember that you can use `\usepackage{parskip}` to change this to an empty line. 

Paragraphs which have similar or connecting content should form a section. Sections can be clearly marked using section headers. 

### A.3. Use correct grammar

#### Do not use colloquial language

You might initially write informally and use some phrases that only exist in spoken language, make sure you fix this in the next edit. For example, in stead of writing `in the \$\mathbb{R}\$`, write `in \$\mathbb{R}\$`.

#### Use words for numbers up to and including twenty.
In Dutch this is standard practice. 

For instance:

<div class="example">
one function, two variables, three subgroups.
</div>

Exception: numbers used as mathematical objects are writting using numbers:

<div class="example">
There are seven partitions of 5.
</div>

#### Make sure to remember Dutch vs English conventions for compound words
In Dutch -- as opposed to in English-- we write compound words joined together, sometimes with a hyphen to connect them if this improves legibility. 

<div class="example">
In Dutch:
differentiaalvergelijking, \$x\$-waarde, computersimulatie.

vs In English:
differential equation, \$x\$ value, computer simulation.
</div>

Make sure to fit your writing style to the language you are writing in.

### A.4. Write introductions and connecting ends
Help your reader by starting every chapter (or section) with an *introduction*, in which you highlight the main takeaway in clear and easy language. For instance, what is the goal of the section, why, and how will you achieve it? You can try and start with a *bridge* to the previous chapters:

<div class="example">
In the previous chapter we saw that \$a\$ is equal to \$b\$. Now we will investigate whether \$a\$ is equal to \$c\$.
</div>

At the end of a chapter you do the same thing with your *closing words*: you state what you have done and where that led. You can also make a bridge to what follows:

<div class="example">
In the following chapters we will apply this result.
</div>

In between definitions and theorems you can also help the reader with introductions and closing words. Explain what you have already done and what you would like to know now. 

These connecting words are usually added in the second edit of the text. That is when you have a clearer idea of how every part is connected. Writing these also helps you think about your text so far. 

### A.5. Be careful when naming things

Chose helpful symbols for your variables. For example, it is standard to use \$n\$ or \$m\$ for integers, and \$f\$ or \$g\$ for functions. It is key that your naming is consistent. Be extra careful with symbols that look similar such as \$1\$ and \$l\$ (you can always use \$\ell\$ (`\ell`) in stead of the letter l. 

Only name objects when you really need to. In the next example, the variable \$N\$ is unnecessary:

<div class="example">
**Theorem A.1.** Every natural number \$N\$ has a unique prime factorisation.
</div>

### A.6. Find a balance between words and symbols

Students of mathematics often write everything in formulas, and do not use regular language much. Compare the following two fragments:

<div class="example">
The greatest common divisor of \$a\$ en \$b\$, written \$\ggd(a, b)\$,
is the largest natural number dividing both \$a\$ and \$b\$.
</div>

<div class="example" markdown="0">
We define: $\ggd(a,b) = {\max{ \{d \in \N_{>0} : d | a \wedge d | b \}} }$.
</div>

The second definition may be shorter, but is it easier to read than the first? Avoid formulas when they are not needed. "A good attitude tothe preparation of written mathematical exposition is to pretend that it
is spoken. Pretend that you are explaining the subject to a friend on a
long walk in the woods, with no paper available." [Halmos]

### A.7. Number equations when needed

Give an equation in a display a number if *and only if* you refer to the number somewhere. We will learn how to do references in LaTeX in <a href="https://uva-fnwi.github.io/LaTeX/week2/maths2/">lesson 11</a>.

### A.8. Give every figure and table a caption

Someone who reads your article or thesis will usually not read it front to back, but skipping through it. Figures and tables are most often the first thing that gets read. Make sure your figures and tables have captions that make sense independent of the rest of the text. You can even move a bit of the explanation in the text to the caption. Exactly how to insert figures into your document we will learn in <a href="https://uva-fnwi.github.io/LaTeX/week3/structure2/">lesson 13</a>.

### A.9. Use displays when it is needed

A mathematical expression in line with the text like \$zeta(s) = \sum_{n=1}^{\infty} n^{-s}\$ is less noticable than the same expression in a display:
\\[
\zeta(s) = \sum_{n=1}^\infty n^{-s}.
\\]

An equation on its own line is called a *display*, and an equation within the line of text is called * inline*. There are several reasons to use display for an equation:

1. The equation is important
2. The equation is referenced
3. The equation is hard to read inline, for example a complicated integral
4. The equation is too big for a line of text, for example a matrix.

If you always use inline expression, you get a very dense text which is difficult to read, unless there are hardly any formulas at all. Display formulas create some air in your text. Do be careful: too many display formulas is like stressing every syllable when you speak. Make sure the balance between inline equations and display expression is good: only use displays when needed. 

An expression which is too big for a line of text can sometimes be rewritten to fit. For example \$\frac{f+2}{f+1}\$ can be replaced by \$(f+2)/(f+1)\$.

### A.10. Use the right layout for definitions and theorems

Important definitions and theorems should be put in their own paragraph which starts with a heading **Definition 1** or something similar. Give your definitions and theorems numbers and make sure your counting method is consistent throughout the text. Usually, people leave empty lines before and after the definition or theorem. In definitions it is common to italicise the concept that is being defined:

<div class="example">
**Definition A.2.** An *even* number is an integer which is divisible by 2.
</div>

Theorems, propositions, lemmas, etc. are traditionally given in italics:

<div class="example">
**Theorem A.3.** *The number \$n^5 - n\$ is divisible by 10 for all
\$n\in\N\$.*
</div>

Use `\emph` t oitalicise the concept in definitions. 

It is far easier not to do this layout yourself but to use the package `amsthm`. In <a href="https://uva-fnwi.github.io/LaTeX/week3/structure2/">esson 14 (week 3) </a> we will learn how to do this. 

B. LaTeX
--------

In this paragraph we will discuss some good rules of thumb for using LaTeX. Many of these rules we have already seen in previous lessons. 

### B.1. Use and make structure commands

The power of LaTeX is the possibilty to give a text structure without fixing the exact layout. A text is structured using commands like

- `\chapter{}`
- `\section{}`
- the `itemize` environment
- `\emph`

Examples of layout commands are

- `\Large`
- `\vspace{}`
- `\textbf{}`
- `\textsl{}`

Only use structure commands in your text. For example, write
```latex
An \emph{even} number is a number which is divisible by 2.
```
and not
```latex
An \textit{even} number is a number which is divisible by 2.
```

The layout of these structural elements can be changed or defined in the preamble. You can make your own structural commands using `\newcommand` there, if you need to.

### B.2. Keep your tex code neat

Writing neat code prevents mistakes and makes it easer to find something again later. A good rule of thumb is to write code like you want the output to look. Here follow a few examples. 

Put commands for a display on separate lines:
```latex
We find
\[
x = 10.
\]
```

Use `\begin` and `\end` commands of environments on seperate lines:

```latex
\begin{equation}
a^2 + b^2 = c^2
\end{equation}
```

Use empty lines between elements of your text. 
```latex
\section{Introduction}
This is an introduction. In an introduction you give a short overview of what this text is about.

\section{Theorem}
Here we give a theorem

\begin{theorem}
There are an infinite number of primes.
\end{theorem}

\begin{proof}
Assume there are $n$ primes.
\end{proof}

\section{Conclusion}
Here we give a conclusion.
```

### B.3. Do not type unecessary empty lines

An empty line in your code is a command; it marks the beginning of a new paragraph. Consider this when using rule B.2.

A common mistake is using an empty line after a display while the paragraph continues. This gives unecessary indents or empty lines. An example of an incorrect use of whitespace is the following

```latex
Consider the symmetric polynomial

\[

(X_1 - X_2)^2.

\]

This is clearly symmetrical.
```
<div class="example" markdown="0">
Consider the symmetric polynomial
\[
(X_1 - X_2)^2.
\]

   This is clearly symmetrical.
</div>

### B.4. Use babel

LaTeX sees any text as an English text by default. This is noticeable from the table of content, captions of figures and tables, and the way words are split and divided over multiple lines. 
If you are writing in Dutch, make sure to use `\usepackage[dutch]{babel}` in the preamble. Notice that when you are using the Dutch version of Babel, this also uses Dutch words in environments like theorem and proof. 

### B.5. Split sentences over multiple lines correctly

A tilde `~` in LaTeX denotes a *non breaking space*. It can be used in place of a space if you do not want the sentence to be cut at that space. For example, this can be used to prevent a symbol from appearing at the beginning of a line: 
```latex
the number~$n$, the function~$f$, the Hilbert space~$H$.
```

You can also use the tilde to neatly display lists of short symbols:
```latex
the variables $x$,~$y$ and~$z$.
```

To give a preference for where an instance of a given word gets split up, you can use `\-`, for instance:
```latex
preferen\-tial
```
If you do this LaTeX will only try and break the word where the `\-` appears and not the other places. If you do want it to consider the other places you can write:
```latex
pref\-er\-en\-tial
```

Within an inline formula you can use braces to denote parts in which you do not want a break. In the expxression `${a^2+b^2}=c^2$` there will not be a break around the `+`. 

If you really do not want any breaks in the middle of an equation, you can put it in an `\hbox{}`. LaTeX will first see this, before the sentence. Note: within an `\hbox{}` mathematical formulas do need to be given between single dollar signs. 

If all these methods still do not give you your desired result, it might be necessary to rewrite your text. Consider changing the word order in your sentence. This may seem like giving up, but in fact it is usually the most practical solution. Do not immediately do this, but wait until you are finishing up the full text. It might happen that the problem solves itself because you've added or removed text which moved the problematic word away from the end of the line. 

### B.6. Avoid double space after period

A period immediately followed by a space is read as the end of a sentence in LaTeX. After each sentence LaTeX automatically adds double space to separate individual sentences more clearly. Usually this is helpful, however when you are using abbreviations or titles you do not want this. To avoid the extra space you can use either the non breaking space `~` or the command for a regular space `\ `. For example: `Dr.~G.F.~Helmink` or `Dr.\ G.F.\ Helmink`.

### B.7. Use `\DeclareMathOperator` for new operators

LaTeX has many built in operators such as `\sin`, `\max`, and `\lim`. To use other operators like for example Tr for the trace of a matrix, you can define your own operator in the preamble.
```latex
\DeclareMathOperator{\Tr}{Tr}
```
This way you separate layout from content and you create the right amount of whitespace around the operator. 


<div class="panel panel-success">
<h3 class="panel-heading panel-title"> Remember </h3>
<div class="panel-body">
* Writing mathematics:
    - Write in full sentences, starting with a capital letter and ending in a period.
    - Divide the text into paragraphs and sections.
    - Write in grammatically correct sentences.
    - Make use of introductions and closing words.
    - Be careful when naming things.
    - Find the right balance between words and symbols.
    - Give equations a number only when this is necessary.
    - Write a caption for your figures and tables.
    - Use displays when needeed.
    - Use the correct layout for theorems and definitions.
* LaTeX:
    - Use (and define) structural commands
    - Keep your code neat.
    - Do not type empty lines or extra spacing when this is not needed.
    - Use Babel.
    - Make sure words are split over lines correctly.
    - Avoid unwanted double whitespace after a period.
    - Use `\DeclareMathOperator` for new operators.

</div> </div>

------------------------------------------------------------------------

### References

1.  Dimitri Bertsekas. [*Ten simple rules for
    mathematical writing.*](http://web.mit.edu/dimitrib/www/Ten_Rules.pdf) 2002.
2.  Edsger W. Dijkstra en A.J.M. van Gasteren.
    [*On naming.*](http://www.cs.utexas.edu/users/EWD/ewd09xx/EWD958.PDF)
    Mei 1986.
3.  David Goss. [*Some Hints on
    Mathematical Style.*](http://www.math.osu.edu/~goss.3/hint.pdf)
4.  Paul R. Halmos. [*How to
    write mathematics.*](http://www.math.uga.edu/~azoff/courses/halmos.pdf)
    American Mathematical Society, 1973.
5.  D.E. Knuth, T. Larrabee en P.M. Roberts.
    [*Mathematical Writing.*](http://tex.loria.fr/typographie/mathwriting.pdf)
    Maa Notes. Mathematical Association of America, 1996.
6.  Andrew D. Lewis. [*Latex do’s
    and don’t’s.*](http://www.mast.queensu.ca/~andrew/LaTeX/latex-dos-and-donts.pdf) 2011.
7.  Jean-Pierre Serre. [*How to write
    mathematics badly.*](http://www.youtube.com/watch?v=tJZpdXWm4Gg) Video.
    2009.
8.  Mark Trettin en Jürgen Fenn. [*An essential guide to LaTeX
    2e usage.*](ftp://ftp.dante.de/tex-archive/info/l2tabu/english/l2tabuen.pdf) 2007.
