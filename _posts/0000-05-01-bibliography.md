---
layout: lesson
title: Bibliography and citations in LaTeX
category: extra1
description: Making a bibliography.
---

Previously we examined the global structure of a LaTeX file and
we have learned how to add more structure to our texts by means 
of chapters, paragraphs, a table of contents, etc. The basic steps
on how to make a reference list are presented in [Week 3](http://uva-fnwi.github.io/LaTeX/week3/structure2/).

In this module we present some more details regarding citations and the list of references.


Reference and citation style for mathematics
--------------------------------------------

<b> Citations </b>
There are many different ways of citing resources from your research. The citation style 
sometimes depends on the academic discipline involved. For example:

<ul>
  <li><a href = "https://pitt.libguides.com/citationhelp/apa7">APA</a> (American Psychological Association) is used by Education, Psychology, and Sciences</li>
  <li><a href = "https://pitt.libguides.com/citationhelp/mla8thedition">MLA</a> (Modern Language Association) style is used by the Humanities</li>
  <li><a href = "https://pitt.libguides.com/citationhelp/chicago">Chicago/Turabian</a> style is generally used by Business, History, and the Fine Arts</li></ul>

For mathematics papers there is no standard citation style, but a good one to learn is the one used by the American Mathematical Society.
The AMS style of in-text citation can simply be a number or an alpha-numeric code. The format depends on the citation style you choose, two examples
that are often used are
<ul>
  <li>[4] - AMS "plain" style; </li>
  <li> [Ma97] - AMS "alpha" style of using first two letters of author's name and last two digits of year of publication. </li>
</ul>

The most common style is a number within brackets, e.g., [1], [2]. The next most common style is a short alpha-numeric form, e.g., [Serre71] or (even
shorter) [S71]. When multiple authors are involved, the citations become lengthy, e.g., [dlVP-SD04] for de la Valleé-Poussin and Swinnerton-Dyer
from 2004. See Chapter 10 from the [AMS Style Guide](https://www.ams.org/publications/authors/AMS-StyleGuide-online.pdf) for more information regarding
the AMS layout style.

In many occassions a specific result is used from a resource. In this case it is nice for the reader if your citation to this resourse is concrete,
for example [4, Thm 3.1] (or [4, Theorem 3.1]) or [Ma97, Thm 3.1]. In LaTeX you can do this as follows: `\cite[Theorem 3.1]{Ma97}`. 

<b> References </b>

The format for your list of sources depends on the citation style you chose, but each entry on the list usually includes the
<ul>
  <li> author's name; </li>
  <li> title of the book or article; </li>
  <li> name of the publisher or journal; </li>
  <li> date of publication; </li>
  <li> pages on which the source material appears.</li>
</ul>

Below you can find some stylistic conventions, some thanks to [Prof. Hildebrand](https://faculty.math.illinois.edu/~hildebr/tex/tips-bibliographies.html), 
regarding your reference list

<ol>
  <li> All items listed in the bibliography should be cited in the body of the paper. There should be no "gratuitious" references.</li>
  <li> Bibliography items should be ordered alphabetically, by author. Multiple references by the same author (or the same set of authors) should be ordered chronologically.</li>
  <li> Be consistent. Whatever format and style you choose, make sure that the same style/format is used for all bibliography entries. Inconsistencies in the bibliography are distracting and create a bad impression on the reader/referee of the paper. For example, first names of authors may be abbreviated or spelled out (most people prefer the former), but whatever choice is made, it should be applied consistently to all references.</li>
  <li> Formatting of bibliography entries. When formatting bibliographies manually with "\bibitem", the following standard conventions should be followed.
      <ol>
          <li> Author(s), title, and journal name. The two most common ways to format these three items are: (i) italics for the title of the paper, and ordinary (Roman) font for the author(s) and the name of the journal; (ii) italics for the name of the journal, and ordinary font for author(s) and title. The examples below illustrate both styles
<div class="example" markdown="0">
  C. O'Cinneide and P. Purdue (1986). <i>The M/M/</i>$\infty$<i>queue in a random environment</i>. Journal of Applied Probability <b> 23</b>, pp. 175-184.
</div>  
<div class="example" markdown="0">
C. O'Cinneide and P. Purdue (1986). The M/M/$\infty$ queue in a random environment. <i>Journal of Applied Probability</i> <b> 23</b>, pp. 175-184.
            </div> </li>
          <li>Volume, issue, year, and page numbers. In contrast to popular magazines, which begin each issue with page number 1, scholarly journals are grouped into volumes, consisting of two or more issues each, and are paginated consecutively within each volume. Thus, an article is (usually) uniquely identified by specifying the volume number (e.g., volume 99) and the page range (e.g., pages 403-422). The particular issue within a given volume need not be specified, and usually (though not always) is left out. A journal may issue one or more volumes per year. The AMS convention is that the year of publication is included in parenthesis after the names of the authors  and the volume and pages are presented after the name of the journal. A typical volume/page number listing is: 99, pp. 403-422.</li>
           <li>Book references. In addition to author and title, book references require the following items: publisher, location, and year of publication. These are normally set in ordinary font, in the order given here.</li></ol>
  <li> Many scientists use arXiv to communicatie their research. arXiv is a free distribution service and an open-access archive for scholarly articles in the fields of physics, mathematics, computer science, quantitative biology, quantitative finance, statistics, electrical engineering and systems science, and economics. Mathematicians use and cite articles from arXiv very often but bear in mind, articles on arXiv are <b>not</b> peer-reviewed and sometimes they contain errors. If you use an article from arXiv be very careful with this. Articles from arXiv should also appear in your reference list using the unique code arXiv attributes to each article. Below you can find two examples on how to properly refer to such articles:
<div class="example" markdown="0">
  C. Radin (2020). <i>Conway and aperiodic tillings </i>. arXiv:2008.09085.
</div>  
<div class="example" markdown="0">
C. Radin (2020). <i>Conway and aperiodic tillings </i>. https://arxiv.org/abs/2008.09085. 
</div> </li></ol>

Trying to typeset <b>URL references</b> manually can be a source of endless frustration since URL's tend to be lengthy "words" that are likely to cause overfull
lines, and also since URL's often contain special symbols (e.g., the "at" symbol "@", the tilde symbol "~", or an "underline", "_") which require special coding in
order to get typeset correctly. For example, the tilde symbol is interpreted by TeX as a "hard" blank space. In order for it to be printed as a tilde symbol, one can
escape it by a backslash (`\~`), or the math "twiddle" symbol $\sim$ in its place, but neither option is completely satisfactory. Fortunately, there is a package,
url, that provides a painless way to typeset URL's. To use this package available, simply add
   
```latex
\usepackage{url}
```
    
near the beginning of the document (after `\documentclass{...}`), and enclose any web and email addresses in the document in `\url{...}`:
    
```latex
\url{http://www.math.drofnats.edu/~gauss}
\url{gauss@math.drofnats.edu}
```
The `\url{...}` command then does all the work: It sets the enclosed expression in the appropriate typewriter style font, it takes care of any necessary linebreaking,
and it chooses break points intelligently (e.g., between components of an address), and it ensures that special symbols such as the tilde symbol or the "at" symbol get
typeset correctly. 

Citing in a proper way
----------------------

In the previous section we discussed how to cite a resource in your main text. When you need to refer to the literature in a text it is important to give a reference to a suitable and well chosen resource and also to make it clear to the reader why you are refering to this specific resource. It is not enough to just give a citation at the end of a sentence, it must be clear to the reader <b>why</b> this specific resource is given and <b>where</b> to look in the resource if needed. As said before there should be no "gratuitious" references in your report/article/book. After your work is finished have a final look at all the citations and the text around it and make sure that someone who reads your text has a clear answer to the following two answers
<ul>
  <li> Why is this reference given at this points? </li>
  <li> Where should I look in this reference if I want to know more about this point? </li>
  </ul>

Below we give some good/poor examples illustrating these two points. 

<div class="example" markdown="0">
Naturally, the set of isotopic knots form an equivalence class on the set of all knots and classification follows [1].
</div>

This citation is rather ambiguous. The reader has only a vague impression of what is discussed in [1]. What is missing is a concrete reference to a result, section or chapter for [1]. The following citation is a good example. 

<div class="example" markdown="0">
All other logical symbols can be seen as abbreviations. To demonstrate these semantics we look at an example from [1, page 1, figure 1.1] (Figure 2.1 in this document).
</div>

A second example where it is ambiguous why a specific citation is given is the following

<div class="example" markdown="0">
An application where neural networks are widely used is pattern recognition with hand writing recognition being a typical example [1, 2].
<ul>
  <li> [1] A. Baldominos, Y. Saez, and P. Isasi (2018). <i>Evolutionary convolutional neural networks: An application to handwriting recognition</i>. Neurocomputing <b>283</b>, pp 38-52.</li>
  <li> [2] M. A. Nielsen (2015). <i>Neural networks and deep learning</i>.</li>
  </ul></div>
 
What is the problem with these two references? First of all the second reference seems very general given the context in which it is given. It is given as a reference to writing recognition while it concerns a much broader topic. Is there a chapter in it concerning hand writing recognition? Or does the autor give a complete overview of the literature on this topic? Hence this citation should be made more concrete. The first reference seems more relevant but still, it is not clear why it is given. A suggestion to improve the text could be the following

<div class="example" markdown="0">
An application where neural networks are widely used is pattern recognition with hand writing recognition being a typical example. For a clear discussion on how neural networks can be applied in this context we refer to [1]. We refer the interested reader to [2] for an overview of some modern techniques for deep learning and their application in pattern recognition.
</div>
