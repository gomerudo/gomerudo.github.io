---
layout: milestone
title: Achmea
description: Data Scientist (Internship)
date-start: 2018-09-01
date-end: 2018-11-30
img: /img/achmea.png
---

As part of the M.Sc. program at the <a href="http://www.tue.nl/en" target="_blank">Eindhoven University of Technology (TU/e)</a>, I worked 3 months for <a href="https://www.achmea.nl" target="_blank">Achmea</a>. The goal of this internship was to develop and apply an <a href="https://www.automl.org" target="_blank">AutoML</a> solution to help the company to come up with better ML models, particularly for fraud detection. I worked under the supervision of Leon Vink, Cyril Cleven, Senna van Iersel, and Peter Diks.

<div class="img_row">
	<img class="col three" src="{{ site.baseurl }}/img/pic-achmea-tilburg.jpg" alt="" title="Achmea's campus at Tilburg"/>
</div>
<div class="col three caption">
	Achmea's campus at Tilburg.
</div>

<br/>
The work was done in three stages. First, we had to research the state-of-the-art on AutoML and identify the most suitable approaches. Second, we had to implement a python package that let the company re-use the technology for other problems they might face in the future. Third, we tested our method on the fraud detection problem to observe the benefits against an already implemented model. In the end, we mentored the BI team on our AutoML solution.

We found that the AutoML solution helped the BI team to find better models. The method, roughly, consisted of a meta-learning module and an evolutionary algorithm. For the meta-learning part, we used a database of meta-features that characterize public datasets, building a meta-space with which one can find the most similar dataset to a new one, and take its model as a possible solution. Later, with the evolutionary algorithm, the candidate models can be fine-tuned and a winner is selected. 

We made the method open source. You can can check it out in the <a href="https://gomerudo.github.io/auto-ml/" target="_blank">website of the project</a> and the <a href="https://github.com/gomerudo/auto-ml" target="_blank">Git repository</a>.
