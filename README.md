# Developing Text Classification Models usin the 20Newsgroups Dataset

The main problem of this project is to build text classificatio models that can accurately classify text samples in to one of the distinct categories. 
The project uses "Twenty Newsgroups" dataset available through scikit-learn at <a href="https://scikit-learn.org/0.19/datasets/twenty_newsgroups.html" target="_blank">https://scikit-learn.org/0.19/datasets/twenty_newsgroups.html</a>

## Research Questions:
<ul>
  <li>How can we create models that classify each text sample into one of multiple labels, where each label represents a category or topic?</li>
  <li> How can we improve the accuracy of multiclass classification for text samples into the appropriate news categories?</li>
  <li>When dealing with real-world data, it is not uncommon that some news categories have more samples than others. What challenges does this class imbalance creates, and are there strategies to make sure our models work well in such situations?</li>
  <li>In the “Twenty Newsgroups” dataset, we have news categories that has significant similarity, such as 'comp.sys.ibm.pc.hardware' and 'comp.sys.mac.hardware'. How does this similarity impact our models, and are there effective solutions for handling data when some news categories closely resemble each other?</li>
  
</ul>

## Tentative Method
<img alt ="Project Method Flow Chart" src="https://github.com/Satomiko/20Newsgroups/blob/main/20%20NewsGroups%20Flow%20Chart.jpg">

<ol>
  <li>Initial analysis</li>
  <li>Create unique subsets for analysis</li>
  <li>Preprocessing</li>
  <li>Exploratory Analysis of each subset</li>
  <li>Feature Exttraction and Dimensionally reduction</li>
  <li>Experimental design</li>
  <li>Modeling</li>
  <li>Evaluation</li>
  <li>Identify the limitation for improvement</li>
</ol>
