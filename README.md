# Coffee Shops in San Francisco: 
## Looking for meaningful, unconventional and unique experiences

The average coffee drinker in the U.S. consumes **3.1 cups of coffee daily** and there are about **100 million of coffee drinkers** in the U.S. Customers are asking more quality and put more attention in details every day. How we can use the information of reviews that people leave about coffee shops to know what they are talking about? Could we analyze coffee blogs to understand what people are looking for in *their experiences*?

This project is the first approach to answer these questions. We study the coffee shops in *San Francisco*, an interesting city with at least 150 years of coffee history, where a lot of specialty coffee shops are emerging every year.

## Contents:
1. Proposal 
- Details on [`Documents/Proposal.pdf`](./Documents/1_Proposal.pdf).

2. Data Extraction
- In this section we apply **web scraping** to different coffee blogs and Yelp to extract customer reviews. Aditionally, we use **FUSION** to get data thought the Yelp's API. Details can be found in [`Documents/Data-Wrangling.pdf`](./Documents/2_Data_Wrangling.pdf)

3. Data Story
- We have a serie of notebooks listed as Sections on [`Data Story`](./Data_Story) folder with story-telling about what we can do with the data available: analysis of **sentiment patterns** of reviews (polarity and subjectivity), creation of a dictionary with key-phrases from one blog as example using **pre-processing common techniques of NLP** (removing stop-words and special characters, expansion of constractions, tokenization and lemmatization) and **TF-IDF** to measure some basic-statistics. 

4. Data Analysis
- An exploratory data analysis inspecting distribution of polarity and subjectivity, **pearson coefficient** between patterns applying **bootstrapping**, testing the *law of primacy in persuasion*, comparative analysis of **cumulative distributions** of customer reviews and blogs and measurement of periods between reviews and how we can determine the positive or negative impact in the frequency of next reviews. Details about this section can be found in [`Documents/Exploratory_Data_Analysis.pdf`](./Documents/3_Exploratory_Data_Analysis.pdf)

5. Milestone Report
- This [`Milestone Report`](./Documents/4_Milestone_Report.pdf) compiles all the previous results describing the problem statement, description of the dataset and initial findings from exploratory analysis.

6. Machine Learning
- In this section we build the definitive dictionary to build feature vectors of similarity and polarity and we use them to train supervised (**XGBoost**, **Random Forest** and **Gradient Boosting**) and unsupervided models (**k-Means**, **Hierarchical Clustering** and **PCA**). Details on [`Documents/Machine_Learning_Report.pdf`](./Documents/5_Machine_Learning_Report.pdf)

7. Presentation and Final Report
- The [`Final report`](./Documents/6_Final_Report.pdf) compiles the complete project, including the most relevant results (collection, wrangling, EDA) and in-depth analysis using machine learning. Additionally, you can see a summarization in the [`Presentation`](./Documents/7_Presentation.pdf) slides deck.


## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites
- [Download Anaconda](https://www.anaconda.com/distribution/).
- Run Anaconda Navigator and launch a jupyter notebook and open the experience-coffee-searcher folder. 
- Using Anaconda Navigator, you can install the following packages:
  - request
  - nltk
  - textblob
  - py-xgboost

Other libraries applied in this project (numpy, scipy, matplotlib, pandas, seaborn, sklearn, re) do not require installation (default packages in anaconda). They only need to be imported in the notebooks.
