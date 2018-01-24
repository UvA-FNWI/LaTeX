---
layout: lesson
title: Nederlandse schrijfgids (Dutch writing guide)
category: week2
description: Nederlandse stijlregels voor wiskunde en LaTeX.
---

<div class="hide">

\[
    \newcommand{\field}[1]{\mathbb{\#1}}
    \newcommand{\Z}{\field Z}
    \newcommand{\N}{\field N}
    \newcommand{\R}{\field R}
    \newcommand{\ideal}[1]{\mathfrak{\#1}}
    \newcommand{\ggd}{\mathrm{ggd}}
    \DeclareMathOperator{\Tr}{Tr}
    \DeclareMathOperator{\ord}{ord}
\]

</div>
In deze les behandelen we vuistregels bij het schrijven van wiskunde. De
eerste paragraaf gaat over het opschrijven van wiskunde in het algemeen.
De vuistregels hiervoor zijn onafhankelijk van LaTeX. De tweede
paragraaf gaat over goed LaTeXen.
Ziehier een <a href="schrijfgids2013.pdf">pdf-versie van de schrijfgids</a>. 

A. Wiskunde opschrijven
-----------------------

Nieuwe wiskunde bedenken is knap, maar het goed opschrijven is net zo
waardevol. Door aandacht te besteden aan de volgende punten help je de
lezer van je tekst enorm.

### A.1. Schrijf zinnen met een hoofdletter en een punt

Een wiskundetekst is niet anders dan elke andere Nederlandstalige tekst.
Een tekst bestaat uit zinnen. Elke zin begint met een hoofdletter en
eindigt met een punt.

Je dient een zin niet te beginnen met een formule. Je zet er woorden
voor:

<div class="example">
Er geldt \$a=1\$. We zien dat \$f(1) = \pi\$.

</div>
Voor symbolen geldt hetzelfde:

<div class="example">
Het getal \$n\$ is belangrijk. De functie \$f\$ is reëel.

</div>
Een zin eindigt altijd met een punt, ook als de zin op een formule
eindigt:

<div class="example" markdown="0">
Neem een geheel getal $n \not= 0$ en definieer

\[
(\Z/n\Z)^* = \{a \in \Z/n\Z : \gcd(a, n) = 1\}.
\]

</div>
Als een zin na een formule doorgaat, schrijf dan een passend leesteken,
bijvoorbeeld een komma:

<div class="example" markdown="0">
Het teken definieert voor $n \geq 2$ een surjectief homomorfisme

\[

\varepsilon : S_n \to \{+1, -1\},

\]

met andere woorden, $\varepsilon(\sigma \tau) =
\varepsilon(\sigma)\varepsilon(\tau)$ voor alle $\sigma,\tau
\in S_n$.

</div>
### A.2. Verdeel de tekst in alinea's en paragrafen

Zinnen die inhoudelijk samenhangen vormen een alinea. Het begin van een
alinea heeft een *inspringing* zodat de lezer ziet dat er een nieuwe
alinea begint. De eerste alinea na een kopje heeft geen inspringing,
omdat daar duidelijk is dat een nieuwe alinea begint.

Alinea's die inhoudelijk samenhangen vormen samen een paragraaf.
Paragrafen kun je van elkaar scheiden met kopjes.

### A.3. Schrijf goed Nederlands

#### Schrijf schrijftaal.

In eerste instantie zal er misschien spreektaal uit je toetsenbord
komen, maar pas dat aan in een volgende redactieslag. Bijvoorbeeld, je
zegt 'in de \$\mathbb{R}^2\$', maar je schrijft 'in \$\mathbb{R}^2\$'.

#### Schrijf telwoorden uit tot en met twintig.

Bijvoorbeeld:

<div class="example">
één functie, twee variabelen, drie ondergroepen.

</div>
Uitzondering: getallen als wiskundige objecten schrijf je met cijfers:

<div class="example">
Er zijn zeven partities van 5.

</div>
#### Schrijf samenstellingen aaneen.

In het Nederlands schrijven we -- anders dan in het Engels --
samenstellingen aan elkaar, met een verbindingsstreepje als dat de
leesbaarheid verbetert:

<div class="example">
differentiaalvergelijking, \$x\$-waarde, kubusopstapeling,
computersimulatie.

</div>
### A.4. Schrijf in- en uitleidingen

Help de lezer door elk hoofstuk te beginnen met een *inleiding*. In een
inleiding vertel je de kern van het verhaal in gewone-mensentaal: wat
wil je bereiken, waarom en hoe. Begin bijvoorbeeld met een *bruggetje*
naar de vorige hoofdstukken:

<div class="example">
In het vorige hoofdstuk zagen we dat \$a\$ gelijk is aan \$b\$. Nu
bekijken we of \$a\$ gelijk is aan \$c\$.

</div>
Aan het eind van een hoofdstuk doe je hetzelfde met een *uitleiding*: je
vertelt wat je gedaan hebt en waar dat toe geleid heeft. Je kunt ook een
bruggetje leggen naar wat volgt:

<div class="example">
In de volgende hoofdstukken gaan we dit resultaat toepassen.

</div>
Ook tussen definities en stellingen kun je de lezer helpen met in- en
uitleidingen. Leg uit wat je gedaan hebt, en wat je nu wilt weten.

Deze in- en uitleidingen schrijf je meestal niet meteen, maar in tweede
instantie. Dat helpt je ook met nadenken over je tekst.

### A.4. Wees zorgvuldig met naamgeving

Kies geschikte symbolen voor je variabelen. Het is bijvoorbeeld
gebruikelijk om gehele getallen met \$n\$ of \$m\$ aan te duiden en
functies met \$f\$ of \$g\$. Het is vooral belangrijk dat de naamgeving
consistent is. Pas ook op met symbolen die op elkaar lijken, zoals \$1\$
en \$l\$ (in dit geval kun je \$l\$ door \$\ell\$ (`\ell`) vervangen).

Geef objecten alleen een naam als dat nodig is. In het volgende
voorbeeld is de variabele \$N\$ overbodig:

<div class="example">
**Stelling A.1.** Elk natuurlijk getal \$N\$ heeft een unieke
factorisatie in priemgetallen.

</div>
### A.5. Vind een balans tussen woorden en symbolen

Wiskundestudenten zijn vaak geneigd alles in formules uit te drukken en
gewonemensentaal te vermijden. Vergelijk:

<div class="example">
De grootste gemene deler van \$a\$ en \$b\$, geschreven \$\ggd(a, b)\$,
is het grootste gehele getal dat zowel \$a\$ als \$b\$ deelt.

</div>
<div class="example">
We definiëren: \$\ggd(a,b) = {\max{ \{d \in \N_{&gt;0} : d | a
\wedge d | b \}} }\$.

</div>
De tweede definitie is weliswaar korter, maar is het beter leesbaar dan
de eerste? Vermijd fomules als ze niet nodig zijn. "A good attitude to
the preparation of written mathematical exposition is to pretend that it
is spoken. Pretend that you are explaining the subject to a friend on a
long walk in the woods, with no paper available." [Halmos]

### A.6. Nummer formules wanneer nodig

Geef een expressie in een display een nummer dan *en slechts dan als* je
het nummer gebruikt in een verwijzing.

### A.7. Geef figuren en tabellen een onderschrift

Iemand die je verslag of scriptie leest, zal dit in eerste instantie
nooit van voor naar achteren doen, maar eerder bladerend. Figuren en
tabellen worden dan het meest bekeken. Zorg daarom voor een onderschrift
dat zich ook zelfstandig laat lezen. Zo nodig verplaats je een deel van
de uitleg van de tekst naar het onderschrift.

### A.8. Gebruik displays als dat nodig is

Een wiskundige expressie in de tekstregel zoals \$\zeta(s) =
\sum_{n=1}^\infty n^{-s}\$ valt minder op dan dezelfde expressie op
een eigen regel:

\\[
\zeta(s) = \sum_{n=1}^\infty n^{-s}.
\\]

We noemen een tekstvak met een expressie op een eigen regel een
*display*. Een expressie in de tekstregel noemen we een *inline*
expressie. Er zijn een aantal redenen om een expressie in een display te
zetten:

1.  de expressie is belangrijk
2.  er wordt naar de expressie verwezen
3.  de expressie is lastig te lezen in een tekstregel, bijvoorbeeld een
    ingewikkelde integraal
4.  de expressie is te groot voor een tekstregel, bijvoorbeeld
    een matrix.

Als je alle formules inline zet, krijg je een 'dichte' tekst die
moeilijk leesbaar is, tenzij je bijna helemaal geen formules hebt.
Formules in display zorgen voor een beetje 'lucht' in je tekst. Maar pas
op: teveel formules in display zetten, is als praten met de klemtoon op
alle lettergrepen. Zorg dus voor een goede balans tussen inline formules
en formules in display: gebruik alleen displays als die nodig zijn (zie
bovenstaande opsomming).

Een expressie die te groot is voor een tekstregel kun je soms anders
schrijven, zodat geen display nodig is. Je kunt bijvoorbeeld de
expressie \$\frac{f+2}{f+1}\$ vervangen door \$(f+2)/(f+1)\$.

### A.9. Geef definities en stellingen de juiste opmaak.

Belangrijke definities en stellingen zet je in een eigen alinea die
begint met een kopje **Definitie 1.** of iets dergelijks. Geef deze
definities en stellingen een nummer en gebruik dezelfde 'teller' door de
hele tekst. Zet voor en na definities en stellingen een witregel. Zet
definities in romeins font en het begrip dat gedefinieerd wordt cursief:

<div class="example">
**Definitie A.2.** Een *even* getal is een getal dat geheel deelbaar is
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

{% highlight latex %}

Een \emph{even} getal is een getal dat geheel deelbaar is door 2.

{% endhighlight %}

niet:

{% highlight latex %}

Een \textit{even} getal is een getal dat geheel deelbaar is door 2.

{% endhighlight %}

De opmaak van de elementen van de structuur regel je in de preamble.
Maak structuurcommando's bij met `\newcommand` als dat nodig is.

### B.2. Houd je texcode netjes

Het schrijven van nette code voorkomt fouten en maakt het gemakkelijker
om later iets terug te vinden. Een vuistregel is de code te schrijven
zoals de uitvoer eruit ziet. We geven een aantal voorbeelden.

Zet de commando's voor een display op aparte regels:

{% highlight latex %}

We vinden
\[
x = 10.
\]

{% endhighlight %}

Zet `\begin` en `\end`-commando's van omgevingen op aparte regels:

{% highlight latex %}

\begin{equation}
\label{eq:pyth}
a^2 + b^2 = c^2
\end{equation}

{% endhighlight %}

In een `align`-omgeving, tabel of matrix zet je de ampersands onder
elkaar:

{% highlight latex %}
\begin{align*}
x &= 1 + 1 + 8 \\
  &= 2 + 8 \\
  &= 10
\end{align*}

{% endhighlight %}

Gebruik lege regels tussen tekstelementen:

{% highlight latex %}

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

{% endhighlight %}

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
{% highlight latex %}

We beschouwen het symmetrische polynoom
\[
(X_1 - X_2)^2.
\]
Dit is ten duidelijkste een symmetrisch polynoom.

{% endhighlight %}

<div class="example" markdown="0">
We beschouwen het symmetrische polynoom

\[

(X_1 - X_2)^2.

\]

        Dit is ten duidelijkste een symmetrisch polynoom.

</div>
{% highlight latex %}

We beschouwen het symmetrische polynoom
\[
(X_1 - X_2)^2.
\]

Dit is ten duidelijkste een symmetrisch polynoom.

{% endhighlight %}

### B.4. Gebruik Babel

LaTeX behandelt een tekst standaard als Engelse tekst. Dat zie je aan de
inhoudsopgave, data, figuren, tabellen, en aan de afbreking van woorden.
Als je een Nederlandse tekst schrijft, gebruik dan
`\usepackage[dutch]{babel}` in de preamble.

### B.5. Breek juist af

De tilde `~` geeft een *non breaking space*. Gebruik de tilde in plaats
van een spatie, als op die spatie niet mag worden afgebroken. Voorkom
bijvoorbeeld dat een symbool op het begin van een regel wordt gezet:

{% highlight latex %}

het getal~$n$, de functie~$f$, de Hilbertruimte~$H$.

{% endhighlight %}

Gebruik de tilde ook om rijtjes korte symbolen netjes af te breken:

{% highlight latex %}

de variabelen $x$,~$y$ en~$z$.

{% endhighlight %}

Om een woord eenmalig op een voorkeursplek af te breken, gebruik je
`\-`, bijvoorbeeld:

{% highlight latex %}

voorkeurs\-behandeling

{% endhighlight %}

LaTeX zal dan alleen op de plek van de `\-` proberen af te breken en op
de andere plekken niet. Als je dat wel wilt, moet je tikken:

{% highlight latex %}

voor\-keurs\-be\-han\-de\-ling

{% endhighlight %}

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

{% highlight latex %}

\DeclareMathOperator{\Tr}{Tr}
\DeclareMathOperator{\ord}{ord}

{% endhighlight %}

Zo scheid je opmaak van inhoud en krijg je de juiste witruimte rondom de
operator.


<div class="panel panel-success">
<div class="panel-heading">
<h3 class="panel-title">
Onthouden

</h3>
</div>
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

</div>
</div>

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
