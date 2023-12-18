---
layout: lesson
title: Nederlandse schrijfgids (Dutch writing guide)
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
The number \$n\$ is important. The function \$f\$ is real. 
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

white is to say, $\varepsilon(\sigma \tau) =
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

### A.6. Vind een balans tussen woorden en symbolen

Wiskundestudenten zijn vaak geneigd alles in formules uit te drukken en
gewonemensentaal te vermijden. Vergelijk:

<div class="example">
De grootste gemene deler van \$a\$ en \$b\$, geschreven \$\ggd(a, b)\$,
is het grootste gehele getal dat zowel \$a\$ als \$b\$ deelt.
</div>

<div class="example" markdown="0">
We definiëren: $\ggd(a,b) = {\max{ \{d \in \N_{>0} : d | a \wedge d | b \}} }$.
</div>

De tweede definitie is weliswaar korter, maar is het beter leesbaar dan
de eerste? Vermijd fomules als ze niet nodig zijn. "A good attitude to
the preparation of written mathematical exposition is to pretend that it
is spoken. Pretend that you are explaining the subject to a friend on a
long walk in the woods, with no paper available." [Halmos]

### A.7. Nummer formules wanneer nodig

Geef een uitdrukking in een display een nummer dan *en slechts dan als* je
het nummer gebruikt in een verwijzing.

### A.8. Geef figuren en tabellen een onderschrift

Iemand die je verslag of scriptie leest, zal dit in eerste instantie
nooit van voor naar achteren doen, maar eerder bladerend. Figuren en
tabellen worden dan het meest bekeken. Zorg daarom voor een onderschrift
dat zich ook zelfstandig laat lezen. Zo nodig verplaats je een deel van
de uitleg van de tekst naar het onderschrift.

### A.9. Gebruik displays als dat nodig is

Een wiskundige uitdrukking in de tekstregel zoals \$\zeta(s) =
\sum_{n=1}^\infty n^{-s}\$ valt minder op dan dezelfde uitdrukking op
een eigen regel:

\\[
\zeta(s) = \sum_{n=1}^\infty n^{-s}.
\\]

We noemen een tekstvak met een uitdrukking op een eigen regel een
*display*. Een uitdrukking in de tekstregel noemen we een *inline*
uitdrukking. Er zijn een aantal redenen om een uitdrukking in een display te
zetten:

1.  de uitdrukking is belangrijk
2.  er wordt naar de uitdrukking verwezen
3.  de uitdrukking is lastig te lezen in een tekstregel, bijvoorbeeld een
    ingewikkelde integraal
4.  de uitdrukking is te groot voor een tekstregel, bijvoorbeeld
    een matrix.

Als je alle formules inline zet, krijg je een 'dichte' tekst die
moeilijk leesbaar is, tenzij je bijna helemaal geen formules hebt.
Formules in display zorgen voor een beetje 'lucht' in je tekst. Maar pas
op: teveel formules in display zetten, is als praten met de klemtoon op
alle lettergrepen. Zorg dus voor een goede balans tussen inline formules
en formules in display: gebruik alleen displays als die nodig zijn (zie
bovenstaande opsomming).

Een uitdrukking die te groot is voor een tekstregel kun je soms anders
schrijven, zodat geen display nodig is. Je kunt bijvoorbeeld de
uitdrukking \$\frac{f+2}{f+1}\$ vervangen door \$(f+2)/(f+1)\$.

### A.10. Geef definities en stellingen de juiste opmaak.

Belangrijke definities en stellingen zet je in een eigen alinea die
begint met een kopje **Definitie 1.** of iets dergelijks. Geef deze
definities en stellingen een nummer en gebruik dezelfde 'teller' door de
hele tekst. Zet voor en na definities en stellingen een witregel. Zet
definities in Romeins lettertype en het begrip dat gedefinieerd wordt cursief:

<div class="example">
**Definitie A.2.** Een *even* getal is een geheel getal dat deelbaar is
door 2.
</div>

Stellingen, proposities, lemma's, etc. worden traditioneel cursief
gezet:

<div class="example">
**Stelling A.3.** *Het getal \$n^5 - n\$ is deelbaar door 10 voor alle
\$n\in\N\$.*
</div>

Belangrijk is dat je niet handmatig de opmaak instelt, maar het
`amsthm`-package gebruikt. We zullen in de volgende les zien hoe dat
moet. Gebruik `\emph` om in definities het gedefinieerde begrip cursief
te zetten.

B. LaTeX
--------

In deze paragraaf bespreken we een aantal goede vuistregels bij het
gebruiken van LaTeX. Veel van deze vuistregels hebben we al eerder
gezien.

### B.1. Gebruik en maak structuurcommando's

De kracht van LaTeX is de mogelijkheid om een tekst structuur te geven
zonder de opmaak vast te leggen. Een tekst krijgt structuur met
commando's als

-   `\chapter{}`
-   `\section{}`
-   de `itemize`-omgeving
-   `\emph{}`.

Opmaakcommando's zijn bijvoorbeeld

-   `\Large`
-   `\vspace{}`
-   `\textbf{}`
-   `\textsl{}`.

Gebruik in de tekst alleen structuurcommando's. Schrijf dus:

```latex
Een \emph{even} getal is een getal dat geheel deelbaar is door 2.
```

niet:

```latex
Een \textit{even} getal is een getal dat geheel deelbaar is door 2.
```

De opmaak van de elementen van de structuur regel je in de preamble.
Maak structuurcommando's bij met `\newcommand` als dat nodig is.

### B.2. Houd je texcode netjes

Het schrijven van nette code voorkomt fouten en maakt het gemakkelijker
om later iets terug te vinden. Een vuistregel is de code te schrijven
zoals de uitvoer eruit ziet. We geven een aantal voorbeelden.

Zet de commando's voor een display op aparte regels:

```latex
We vinden
\[
x = 10.
\]
```

Zet `\begin` en `\end`-commando's van omgevingen op aparte regels:

```latex
\begin{equation}
\label{eq:pyth}
a^2 + b^2 = c^2
\end{equation}
```

In een `align`-omgeving, tabel of matrix zet je de ampersands onder
elkaar:

```latex
\begin{align*}
x &= 1 + 1 + 8 \\
  &= 2 + 8 \\
  &= 10
\end{align*}
```

Gebruik lege regels tussen tekstelementen:

```latex
\section{Inleiding}
Dit is een inleiding. In een inleiding vertel je kort waar de tekst over
gaat.

\section{Stelling}
Hier geven we een stelling.

\begin{stelling}
Er zijn oneindig veel priemgetallen.
\end{stelling}

\begin{proof}
Stel er zijn eindig veel priemgetallen.
\end{proof}

\section{Conclusie}
Hier staat een conclusie.
```

Het gedeelte van de code voor `\begin{document}` heet de *preamble*.
Nieuwe commando's definieer je in de preamble. Ingewikkelde commando's
licht je toe met commentaar.

### B.3. Typ geen lege regel als dat niet moet

Een lege regel in je code is een commando; het markeert het begin van
een nieuwe paragraaf. Houd hier rekening mee bij het toepassen van B.2.

Een veelgemaakte fout is het schrijven van een witregel na een display
terwijl de alinea doorloopt. Het resultaat is een onterechte inspringing
(onder).

<div class="example" markdown="0" >
We beschouwen het symmetrische polynoom
\[
(X_1 - X_2)^2.
\]
Dit is ten duidelijkste een symmetrisch polynoom.
</div>

```latex
We beschouwen het symmetrische polynoom
\[
(X_1 - X_2)^2.
\]
Dit is ten duidelijkste een symmetrisch polynoom.
```

<div class="example" markdown="0">
We beschouwen het symmetrische polynoom

\[

(X_1 - X_2)^2.

\]

        Dit is ten duidelijkste een symmetrisch polynoom.
</div>

```latex
We beschouwen het symmetrische polynoom
\[
(X_1 - X_2)^2.
\]

Dit is ten duidelijkste een symmetrisch polynoom.
```

### B.4. Gebruik Babel

LaTeX behandelt een tekst standaard als Engelse tekst. Dat zie je aan de
inhoudsopgave, data, figuren, tabellen, en aan de afbreking van woorden.
Als je een Nederlandse tekst schrijft, gebruik dan
`\usepackage[dutch]{babel}` in de preamble.

### B.5. Breek juist af

De tilde `~` geeft een *non breaking space*. Gebruik de tilde in plaats
van een spatie, als op die spatie niet mag worden afgebroken. Voorkom
bijvoorbeeld dat een symbool op het begin van een regel wordt gezet:

```latex
het getal~$n$, de functie~$f$, de Hilbertruimte~$H$.
```

Gebruik de tilde ook om rijtjes korte symbolen netjes af te breken:

```latex
de variabelen $x$,~$y$ en~$z$.
```

Om een woord eenmalig op een voorkeursplek af te breken, gebruik je
`\-`, bijvoorbeeld:

```latex
voorkeurs\-behandeling
```

LaTeX zal dan alleen op de plek van de `\-` proberen af te breken en op
de andere plekken niet. Als je dat wel wilt, moet je tikken:

```latex
voor\-keurs\-be\-han\-de\-ling
```

In een formule die tussen enkele dollartekens staat, kun je met
accolades een afbreekvoorkeur aangeven: `${a^2+b^2}=c^2$`. De accolades
zorgen ervoor dat er niet rond de `+` wordt afgebroken.

Als je echt niet middenin een formule wilt afbreken, zet die dan in een
`\hbox{}`. LaTeX zet eerst die `\hbox{}`, daarna pas de zin. Let op: in
een `\hbox{}` moet een wiskundeformule weer opnieuw tussen enkele
dollartekens.

Als het dan nog steeds niet lukt, ga dan je tekst herschrijven. Keer
bijvoorbeeld de volgorde van een zin om. Dit lijkt misschien op opgeven,
maar is vaak de meest praktische oplossing. Doe dit niet meteen, maar
later -- als je je tekst aan het afronden bent. Het kan immers voorkomen
dat het probleem zichzelf oplost doordat teksten gaandeweg het
schrijfproces nog verschuiven.

### B.6. Voorkom een onjuiste grote spatie na een punt

Een punt met een spatie erna wordt door LaTeX opgevat als het einde van
een zin. De spatie na de punt krijgt een grotere horizontale ruimte dan
een gewone spatie.

De grotere spatie na een punt is meestal goed, behalve bijvoorbeeld in
titulatuur en afkortingen. Om grote spaties te voorkomen, schrijf je
`Dr.~G.F.~Helminck` of `Dr.\ G.F.\ Helminck`. De `~` is een non breaking
space, de `\␣` geeft een gewone spatie, maar het voorkomt wel dat LaTeX
het patroon punt-spatie ziet.

### B.7. Gebruik `\DeclareMathOperator` voor nieuwe operatoren.

Voor het zetten van operatoren als \$\operatorname{Tr}\$ of \$\operatorname{ord}\$ maak je zelf
een operator met

```latex
\DeclareMathOperator{\Tr}{Tr}
\DeclareMathOperator{\ord}{ord}
```

Zo scheid je opmaak van inhoud en krijg je de juiste witruimte rondom de
operator.


<div class="panel panel-success">
<h3 class="panel-heading panel-title"> Onthouden </h3>
<div class="panel-body">
* Wiskunde schrijven:
    - Schrijf zinnen met een hoofdletter en een punt.
    - Verdeel de tekst in alinea's en paragrafen.
    - Schrijf goed Nederlands.
    - Schrijf in- en uitleidingen.
    - Wees zorgvuldig met naamgeving.
    - Vind een balans tussen woorden en symbolen.
    - Nummer formules alleen als dat nodig is.
    - Geef figuren en tabellen een onderschrift.
    - Gebruik displays als dat nodig is.
    - Geef definities en stellingen de juiste opmaak.
* LaTeX:
    - Gebruik en maak structuurcommando's
    - Houd je code netjes.
    - Typ geen lege regel als dat niet moet.
    - Gebruik Babel.
    - Breek juist af.
    - Voorkom een onjuiste spatie na een punt.
    - Gebruik `\DeclareMathOperator` voor nieuwe operatoren.

</div> </div>

------------------------------------------------------------------------

### Referenties

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
