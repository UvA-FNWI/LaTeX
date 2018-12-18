---
layout: lesson
title: Structure
category: week2
description: Structure of a LaTeX file, document classes, packages, topmatter, groups, commands and environments.
---
This lesson is about the structure of a LaTeX file.

A LaTeX document
----------------

Every LaTeX document has the following structure:

<pre><code class='tex'>\documentclass[a4paper]{article}
\begin{document}
\end{document}
</code></pre>

In this, `article` can be replaced by a different *document class*. The
part before `\begin{document}` is called the **preamble**.
The preamble contains commands which influence the entire document. For
example, packages are loaded here. The actual text of your document is
between `\begin{document}` and `\end{document}`.

### Document classes

A **document class** is a collection of settings corresponding to a
specific type of document. The document class is set with

<pre><code class='tex'>\documentclass[options]{class}
</code></pre>

where `options` is a list of options seperated by commas. Later, we will
look further into this.

### Packages

Packages are extensions of LaTeX that add functionality. One can think
of the possibility to add figures or additional commands for
mathematical symbols. Modern *TeX distributions* (see [Installing
LaTeX]({{site.baseurl}}{% post_url 0000-01-01-installinglatex %}))
contain many packages, which can be used by putting

<pre><code class='tex'>\usepackage[options]{packagename}
</code></pre>

in the preamble, with `packagename` the name of the package and
`options` a list of options. A package which is indispensible in Dutch
documents is

<pre><code class='tex'>\usepackage[dutch]{babel}
</code></pre>

The `babel` package with the option `dutch` will make sure that LaTeX
replaces standard titles such as *Chapter* and *Table of contents* by
the Dutch equivalents *Hoofdstuk* and *Inhoudsopgave* respectively. The
package also configures hyphenation so it is essential to use the right
language option.

### Top matter

The preamble is followed by the document environment, beginning with
`\begin{document}` and ending with `\end{document}`. In the first lines
of the document environment one gives information about the document
itself, such as the name of the author, the title and the date. This is
called *top matter*. With the command `\maketitle` LaTeX will typeset
the topmatter following the style of the document class. An example of
top matter is

<pre><code class='tex'>\title{A new proof of an old theorem}
\author{Jane Doe}
\maketitle
</code></pre>
A date can be inserted with `\date{January 1st, 2017}`. If you don't use
`\date`, LaTeX will typeset the current date. More than one author can
be typeset with `\and`:

<pre><code class='tex'>\author{Jane Doe \and John Doe}
</code></pre>

<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">
Exercise 1

</h3>
</div>
<div class="panel-body">
1.  Writing as little code as possible, create a Dutch document with
    title "Een bewijs van de Riemannhypothese" with yourself as
    the author.
2.  Make sure LaTeX typesets the date in Dutch and not in English.
3.  Ask one of the teachers to check your document.

</div>
</div>
<div class="panel panel-danger">
<div class="panel-heading">
<h3 class="panel-title">
Important

</h3>
</div>
<div class="panel-body">
We see that LaTeX determines the layout itself. This is an important
concept in LaTeX! We determine the layout of the text by structuring it.
By seperating layout and content

-   We can focus on the content.
-   We obtain a consistent layout.
-   We (or a publisher) are able to change the layout easily.

</div>
</div>

Structuring text
----------------

In LaTeX we have *groups*, *commands* and *environments* to structure
our document.

### Groups

A **group** is a block of code surrounded by `{` and `}`. A group
indicates that the code belongs together.

### Commands

Examples of commands are `\documentclass`, `\usepackage` and `\author`.
A **command** comes in one of these two types:

-   First a `\` and then a name consisting only of letters. After the
    name a space, a number or a special character follows.
-   First a `\` and then a number or a special character.

The name of a command is case sensitive. Some commands require one or
more arguments, which are written between `{` and `}` after the command.
An argument can be optional, which is indicated by `[` and `]` after the
command. The general syntax is:

<pre><code class='tex'>\commandname[option1,option2,...]{argument1}{argument2}...
</code></pre>

### Environments

An **environment** such as `document` is created by two commands:

<pre><code class='tex'>\begin{name}
\end{name}
</code></pre>

Inside an environment one can write LaTeX code. An environment defines a
group automatically.

<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">
Exercise 2

</h3>
</div>
<div class="panel-body">
In this assignment we will define our own command.

1.  Create a new LaTeX file using the mathtools package and put the
    following in the preamble:

	<pre><code class='tex'>\newcommand{\R}{\mathbb{R}}
	</code></pre>

2.  Test your new command:

	<pre><code class='tex'>The real line $\R{}$.
	</code></pre>

3.  What happens if you remove the empty group `{}`?

4.  We will now create a command with an argument. Put the following in
    the preamble:

	<pre><code class='tex'>\newcommand{\Bb}[1]{\mathbb{#1}}
	</code></pre>

5.  Test it using this code:

	<pre><code class='tex'>The rationals $\Bb{Q}$.
	</code></pre>

6.  With `[1]` we indicate that the command expects a single argument.
	We use this argument with `#1`. Try to make a command with two
	arguments.

</div>
</div>
<div class="panel panel-success">
<div class="panel-heading">
<h3 class="panel-title">
Remember

</h3>
</div>
<div class="panel-body">
-   What is the global structure of a LaTeX file?
-   What do `\documentclass`, `\usepackage`, `\title`, `\author`,
    `\and`, `\date` and `\maketitle` do?
-   What does the `babel`-package do?
-   Why do we seperate layout and content?
-   What are groups, commands and environments?
-   How do you make your own command?

</div>
</div>
