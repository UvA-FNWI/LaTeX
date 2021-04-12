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

**Citations**

There are many different ways of citing resources from your research. The citation style 
sometimes depends on the academic discipline involved. For example:

1.  [APA](https://pitt.libguides.com/citationhelp/apa7) (American Psychological Association) is used by Education, Psychology, and Sciences
2.  [MLA](https://pitt.libguides.com/citationhelp/mla8thedition) (Modern Language Association) style is used by the Humanities
3.  [Chicago/Turabian](https://pitt.libguides.com/citationhelp/chicago) style is generally used by Business, History, and the Fine Arts

For mathematics papers there is no standard citation style, but a good one to learn is the one used by the American Mathematical Society.
The AMS style of in-text citation can simply be a number or an alpha-numeric code. The format depends on the citation style you choose, two examples
that are often used are the following.

The most common style is a number within brackets, e.g., [1], [2]. The next most common style is a short alpha-numeric form, e.g., [Serre71] or (even
shorter) [S71]. When multiple authors are involved, the citations become lengthy, e.g., [dlVP-SD04] for de la Valleé-Poussin and Swinnerton-Dyer
from 2004. See Chapter 10 from the [AMS Style Guide](https://www.ams.org/publications/authors/AMS-StyleGuide-online.pdf) for more information regarding
the AMS layout style.

In many occassions a specific result is used from a resource. In this case it is nice for the reader if your citation to this resourse is concrete,
for example [4, Thm 3.1] (or [4, Theorem 3.1]) or [Ma97, Thm 3.1]. In LaTeX you can do this as follows: `\cite[Theorem 3.1]{Ma97}`. An example is given
below

<div class="example" markdown="0">
<b>Theorem</b> (Theorem 2.3, [1])
For every $p \in (0,1)$, the sequence of probability distributions $(\tilde{\mathbb{P}}_{n,p})_{n\in\mathbb{N}}$ 
satisfies the large deviation principle on $(\tilde{W},\delta_{\square})$ with rate function $I_p$, i.e.,
\begin{equation}
\begin{aligned}
\limsup_{n\to\infty} \frac{1}{n^2}\, \log\tilde{\mathbb{P}}_{n,p}(\tilde{C}) 
&\leq -\inf_{\tilde{h}\in\tilde{W}}I_p(\tilde{h}) \qquad \forall\,\tilde{C}\subset \tilde{W} \mbox{ closed},\\
\liminf_{n\to\infty}\ \frac{1}{n^2}\, \log\tilde{\mathbb{P}}_{n,p}(\tilde{O})
&\geq -\inf_{\tilde{h}\in\tilde{O}}I_p(\tilde{h}) \qquad \,\,\,\forall\,\tilde{O}\subset \tilde{W} \mbox{ open}.
\end{aligned}
\end{equation}
</div>


**References**

The format for your list of sources depends on the citation style you chose, but each entry on the list usually includes the

1. author's name; 
2. title of the book or article; 
3. name of the publisher or journal; 
4. date of publication; 
5. pages on which the source material appears.

Below you can find some stylistic conventions, some thanks to [Prof. Hildebrand](https://faculty.math.illinois.edu/~hildebr/tex/tips-bibliographies.html), 
regarding your reference list

1. All items listed in the bibliography should be cited in the body of the paper. There should be no "gratuitious" references.
2. Bibliography items should be ordered alphabetically, by author. Multiple references by the same author (or the same set of authors) should be ordered chronologically.
3. Be consistent. Whatever format and style you choose, make sure that the same style/format is used for all bibliography entries. Inconsistencies in the bibliography are distracting and create a bad impression on the reader/referee of the paper. For example, first names of authors may be abbreviated or spelled out (most people prefer the former), but whatever choice is made, it should be applied consistently to all references.
 4. Formatting of bibliography entries. When formatting bibliographies manually with "\bibitem", the following standard conventions should be followed. 
      1. Author(s), title, and journal name. The two most common ways to format these three items are: (i) italics for the title of the paper, and ordinary (Roman) font for the author(s) and the name of the journal; (ii) italics for the name of the journal, and ordinary font for author(s) and title. The examples below illustrate both styles
      2. Volume, issue, year, and page numbers. In contrast to popular magazines, which begin each issue with page number 1, scholarly journals are grouped into volumes consisting of two or more issues each, and are paginated consecutively within each volume. Thus, an article is (usually) uniquely identified by specifying the volume number (e.g., volume 99) and the page range (e.g., pages 403-422). The particular issue within a given volume need not be specified, and usually (though not always) is left out. A journal may issue one or more volumes per year. The AMS convention is that the year of publication is included in parenthesis after the names of the authors  and the volume and pages are presented after the name of the journal. A typical volume/page number listing is: 99, pp. 403-422.
      3. Book references. In addition to author and title, book references require the following items: publisher, location, and year of publication. These are normally set in ordinary font, in the order given here.
  5. Many scientists use arXiv to communicatie their research. arXiv is a free distribution service and an open-access archive for scholarly articles in the fields of physics, mathematics, computer science, quantitative biology, quantitative finance, statistics, electrical engineering and systems science, and economics. Mathematicians use and cite articles from arXiv very often but bear in mind, articles on arXiv are <b>not</b> peer-reviewed and sometimes they contain errors. If you use an article from arXiv be very careful with this. Articles from arXiv should also appear in your reference list using the unique code arXiv attributes to each article. Below you can find two examples on how to properly refer to such articles:
     1. C. Radin (2020). *Conway and aperiodic tillings*. arXiv:2008.09085.
     2. C. Radin (2020). *Conway and aperiodic tillings*. https://arxiv.org/abs/2008.09085.

**Typesetting online resources**

Nowadays most new scientific articles can be found online and it is important to be able to find them there quickly as well. One means for this is the Digital Object Identifier, or DOI. A DOI is a unique and permanent code that is linked to a specific source, for example 10.1016 / j.jcss.2007.06.005. Place this code after http://dx.doi.org/ and a link will appear leading to the article, such as http://dx.doi.org/10.1016/j.jcss.2007.06.005. This code is assigned and updated when necessary by a publisher - so it is not just possible to link a DOI to your own work.

If a source has a DOI, always mention it in the reference list. If it does not have a DOI but is online, please provide a URL. The disadvantage of a URL is that the location of an article can change and thus the URL no longer leads to the source, while the link of the DOI is updated. If a source has been consulted online that can be adjusted later, it must state the date on which it was consulted or, if stated, the date on which the last adjustment took place. In general, this does not apply to scientific articles, but to sources such as a blog or Wikipedia.

Trying to typeset URL references manually can be a source of endless frustration since URL's tend to be lengthy "words" that are likely to cause overfull
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
