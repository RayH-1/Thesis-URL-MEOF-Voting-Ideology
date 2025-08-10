# Code for Master's Thesis at the Hertie School of Governance

---

The goal of this project is to determine if the digital trace information and personal demographic information can be used to predict whether an individual will vote for a specific party in an upcoming election. If not, the goal then is to determine if the same information can deduce voter ideology. It builds on existing research by looking at news sources, specifically headlines, at the URL and individual levels. 

The code can be broken up into various sections:
**Initial Data Cleaning and Exploratory Data Analysis (EDA)**
1. `00_Data_Check.Rmd`
2. `01_Data_Columns.Rmd`
3. `02_Tracking_Cleaning.Rmd`
4. `03_Survey_Tracking_Merging.Rmd`
5. `04_Simple_Models.Rmd`: Includes running simple linear regression on demographic information.

**Natural Language Processing**
1. `05_TF-IDF.ipynb`
2. `08_TopicLDA_Bayes.ipynb`: Topics are "generated" using Latent Dirichlet Allocation.
3. `09_1_LDA_Exploration_Ideology.ipynb`: LDA is checked on data at the URL level (each domain is a unique row).
4. `09_2_LDA_Exploration.ipynb`: LDA is checked on the data at the person level (each person is a unique row).

**Machine Learning Models**
1. `06_1_LinearSVC.ipynb`: This includes some EDA of the topics, but the machine learning focuses on the output variable `left_right`, which is the ideological categorization.
2. `06_2_LinearSVC_Party.ipynb`: This looks at the `secondvote` variable, which is the party categorization.
3. `07_1_Traditional_Models_Ideology.ipynb`: Models include Logistic Regression, Random Forest, Decision Trees, Support Vector Machine, and Gradient Boosting.
4. `07_2_Traditional_Models_Parties.ipynb`
5. `08_TopicLDA_Bayes.ipynb`: Bayes's is used to determine any topics that correlate with the classes (party ideology and party vote).
6. `10_1_MLP_Ideology.ipynb`: Small multilayer perceptron 
7. `10_2_MLP_Party.ipynb`

**Dropped Code/Attempted Code (For Testing Purposes)**
1. `D7_XGBoost_Featureselection_Models.ipynb`
2. `D8_BERTopic.ipynb`: Abandoned due to lack of compute resources. This would have taken too long, so LDA was settled on. 



# Artificial Intelligence Disclosure
---
AI is used to bug-fix code chunks where necessary. The tools used were ChatGPT, Claude, and DeepSeek. 
