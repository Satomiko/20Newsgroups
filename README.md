# Developing Text Classification Models using the 20Newsgroups Dataset

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
<li><b>Initial Analysis:</b> Conduct univariate analysis to understand the original data.</li>
<li><b>Subset Creation:</b> Create 3 subsets to assess the impact of text data characteristics on performance. In each subset, select 5 out of 20 available categories strategically. The first subset comprises 1 category from each of the different main topic, while the second subset includes five categories all related to a single topic. Additionally, create a third subset by combining small classes within the main topics, intentionally introducing an imbalance in this subset.</li>
<li><b>Data Preprocessing:</b>Clean the text data by performing the following techniques:
  <ul>
<li>Lowercasing</li>
<li>Removing stop words</li>
<li>Removing special characters</li>
<li>Lemmatization</li> 
<li>Removing one-letter words</li>
<li>Deleting empty observations</li></ul>
</li>
  <li><b>Exploratory Analysis:</b>Identify frequent words for each class by using word cloud. The 10 most frequent words for each class are identified.</li>
  <li><b>Feature Extraction and Dimensionality Reduction:</b> TF-IDF (Term Frequency-Inverse Document Frequency) technique is used to extract features from the text data. In this study, dimension of the data is controlled using the “max_features” argument within the “Tfidvectorier” functions.</li>
  <li><b>Experimental Design and modeling:</b> Apply Multinomial Naive Bayes, Decision Tree, Logistic Regression, and Support Vector Machine for predictive modeling. The 20 news group data set is pre-separated into training and testing sets. Cross-validation is performed on training data.</li>
  <li><b>Evaluation:</b> Assess model performance using confusion matrix, precision, accuracy, and recall. Compare performance across machine learning algorithms and as well as across subsets.</li>
  <li><b>Conclusion:</b> Identifying the limitations of the models, which will serve as a foundation for future improvements.</li>
</ol>

## Contents of Repository:
<ul>
<li>  Flow Chart showing method of project: <a href='https://github.com/Satomiko/20Newsgroups/blob/main/20%20NewsGroups%20Flow%20Chart.jpg'>20 NewsGroups Flow Chart.jpg</a></li>
<li> Select Preprocessing Method after review:<a href='https://github.com/Satomiko/20Newsgroups/blob/main/2_preprocessing_methods.ipynb'>2_preprocessing_methods.ipynb</a></li>
<li> Working Python code for initial Anaylsis of Original Dataset:<a href='https://github.com/Satomiko/20Newsgroups/blob/main/Original_20_Newsgroup_Data.ipynb'>Original_20_Newsgroup_Data.ipynb</a></li>
<li> Working Python code for initial Anaylsis of Original Dataset (PDF): <a href='https://github.com/Satomiko/20Newsgroups/blob/main/Original_20_Newsgroup_Data.pdf'>Original_20_Newsgroup_Data.pdf</a></li>
<li> Working Python code for creating subsets, preprocessing, exploratory Analysis, Feature extraction, Ecperimental design, Modeling and Evaluation: <a href='https://github.com/Satomiko/20Newsgroups/blob/main/Subsets_Experiment_and_Analysis.ipynb'>Subsets_Experiment_and_Analysis.ipynb</a></li>
<li> Working Python code for creating subsets, preprocessing, exploratory Analysis, Feature extraction, Ecperimental design, Modeling and Evaluation (PDF): <a href='https://github.com/Satomiko/20Newsgroups/blob/main/Subsets_Experiment_and_Analysis.pdf'>Subsets_Experiment_and_Analysis.pdf</a> </li>

</ul>
All .ipynb files in this project were created using Colaboratory. 

