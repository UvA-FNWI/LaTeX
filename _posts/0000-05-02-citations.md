---
layout: lesson
title: Bibliography and citations in LaTeX
category: extra1
description: Proper citations in the text.
---

Citing in a proper way
----------------------

In the previous section we discussed how to cite a resource in your text. When you need to refer to the literature in a text it is important to give a reference to a suitable and well chosen resource. It is also important to make clear to the reader why you are refering to a certain resource. It is not enough to just give a citation at the end of a sentence, it must be clear to the reader <b>why</b> this specific resource is given and <b>where</b> to look in it if needed. As said before, there should be no "gratuitious" references in your report/article/book. After you are finished with writing have a final look at all the citations, make sure that someone who reads your text has a clear answer to the following two questions
<ul>
  <li> Why is this specific reference given at this point? </li>
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

A second example where it is ambiguous why a specific citation is given, is the following

<div class="example" markdown="0">
An application where neural networks are widely used is pattern recognition with hand writing recognition being a typical example [1, 2].
<ul>
  <li> [1] A. Baldominos, Y. Saez, and P. Isasi (2018). <i>Evolutionary convolutional neural networks: An application to handwriting recognition</i>. Neurocomputing <b>283</b>, pp 38-52.</li>
  <li> [2] M. A. Nielsen (2015). <i>Neural networks and deep learning</i>.</li>
  </ul></div>
 
What is the problem with these two references? First of all, the second reference seems very general given the context in which it is given. It is given as a reference to " " "writing recognition", while it concerns a much broader topic. The reader may wonder, Is there a chapter in it concerning hand writing recognition? Or does the autor give a complete overview of the literature on this topic? Hence this citation should be made more concrete. The first reference seems more relevant but still, it is not clear why it is given. A suggestion to improve the text could be the following

<div class="example" markdown="0">
An application where neural networks are widely used is pattern recognition, with hand writing recognition being a typical example. For a clear exhibition on how neural networks can be applied in this context we refer to [1]. We refer the interested reader to [2] for an overview of some modern techniques for deep learning and their application in pattern recognition.
</div>
