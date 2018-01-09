---
layout: lesson
title: Hello world!
category: week1
description: Typesetting your first document in TeXworks.
---
This lesson is about what LaTeX is and how to use it.

What is LaTeX?
--------------

LaTeX is used to typeset scientific documents. It is based on the
programming language TeX, which is designed for writing mathematical
texts. There are fundamental differences between LaTeX and other word
processors such as MS Word and Pages.

##### Pros

-   One can concentrate on the structure and content of the document,
    without worrying about the layout.
-   The layout is consistent.
-   Mathematical expressions can be inserted easily.
-   It is easy to number and refer to equations.
-   One is forced to structure every document well.

##### Cons

-   In most editors is not possible to see the result of your
    code immediately.
-   One has to learn LaTeX commands.
-   Some layout elements cannot be edited easily.

The approach LaTeX used is called *What You See Is What You Mean*; when
writing the document you can't see the final result. Instead you see the
structure of the document.

Using LaTeX
-----------

In this course you will learn to work with TeXworks. However, everything
you learn about LaTeX itself is independent of your LaTeX editor.

TeXworks
:   A simple editor which is included in the LaTeX distributions MikTeX
    and TeX Live.

ShareLaTeX
:   An online editor where you can collaborate with others. It is
    convenient to use this on computers where LaTeX isn't installed.

In the first exercise we will assume that you use TeXworks. To install
this, see [Installing LaTeX]({{site.baseurl}}{% post_url 0000-01-01-installinglatex %}.

<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">
Exercise 1

</h3>
</div>
<div class="panel-body">
1.  Open 'TeXworks' on your computer.
2.  Paste the following code in an empty document and save it as
    'helloworld.tex'. The extension of a TeX file always is '.tex'.

	<pre><code class='tex'>\documentclass[a4paper]{article}
\begin{document}
Hello world!
\end{document}</code></pre>

3. Select 'pdfLaTeX' in the menu to the right of the green button and
press the green button afterwards. We call this *typesetting*. LaTeX
turns your code into a PDF document which you will see in a new window.

-   Useful: Select 'Format -> Syntax Coloring -> LaTeX' to colour
    your code.
-   Useful: To jump from the code to the output in TeXworks you can
    right-click and choose 'Jump to PDF'. In the same way it is possible
    to switch from the pdf to the code.

</div>
</div>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">
Exercise 2 (optional)

</h3>
</div>
<div class="panel-body">
1.  Create a [ShareLaTeX-account](https://www.sharelatex.com).
2.  Click on 'New Project' and choose 'Blank Project'. Name your project.
3.  On the left side you see your LaTeX code. Click on 'Recompile' to see the output.

-   Watch out: ShareLaTeX ignores many errors and tries to create a pdf, even when there are mistakes in the LaTeX-code. You can see the errors and warning in 'Logs'

</div>
</div>
From now on you can use any editor you prefer. However, on the final
exam TeXworks must be used.

Resources
---------

We encourage you to use not only this website, but also other resources
if you can't figure something out yourself. The following websites
provide useful information:

[LaTeX Wikibooks](https://en.wikibooks.org/wiki/LaTeX)
:   An up-to-date collection of articles about LaTeX.

[TeX - LaTeX Stack Exchange](http://tex.stackexchange.com)
:   A question and answer site with many active users.

[Detexify](http://detexify.kirelabs.org/classify.html)
:   A symbol recogniser: draw a symbol and it returns the LaTeX command.

<div class="panel panel-success">
<div class="panel-heading">
<h3 class="panel-title">
Remember

</h3>
</div>
<div class="panel-body">
- How to open TeXworks (or ShareLaTeX)?
- How to compile a LaTeX file?
- Don't be afraid to explore the web!

</div>
</div>
