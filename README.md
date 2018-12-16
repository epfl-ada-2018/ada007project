# Title
Title: **How people view health care products？**

Team members: Liang Yueran, Luo Yaxiong, Xia Shengzhao

Data Story: [How people view health care products?](https://ada007project.github.io)

# Abstract

Improving health condition is an indispensable part of society improvement. In this project, we focus on the Amazon product data to draw a conclusion on how to promote health. Our goal is to analyze the popularity of products related to physical health from different points of views, such as providing a visualization of data to show the changing trend of the amount of reviews,  comparing average rating of the products and so on. We hope to give people an insight of how these products influence people’s life. Are they becoming more and more important to people's life or people are losing their interests of these kinds of products? Morever, good recommendations are essential to promote these products for people interested in them. By combining rating, sentiment analysis of reviews and other useful features of data, we also want to make a reasonable recommendation.

# Research questions

* How to define the popularity of healthy products specifically?

* What's the most popular Healthy product? How the average of rating varies between different categories?

* How the ratings of healthy product change and how people rate for different healthy products?

* what are the keywords in reviews for several popular healthy products?

* How to combine serveral features of data such as ratings and reviews to give recommendations?

# Dataset

The primary dataset that we would like to use is the [Amazon Review Dataset](http://jmcauley.ucsd.edu/data/amazon/). This dataset includes reviews (ratings, text, helpfulness votes), product metadata (descriptions, category information, price, brand, and image features)

### Category 

We will mainly concern several category listed below:
* Category information
    * Health & Personal Care
    * ~~Sports & Outdoors~~（because we found even if we do analysis on both two, we will draw two irrelevant conclusions after we analyse them in the same way.)

### Dataset Structure/Format

* Review Dataset
    * reviewerID - ID of the reviewer, e.g. A2SUAM1J3GNN3B
    * asin - ID of the product, e.g. 0000013714
    * reviewerName - name of the reviewer
    * helpful - helpfulness rating of the review, e.g. 2/3
    * reviewText - text of the review
    * overall - rating of the product
    * summary - summary of the review
    * unixReviewTime - time of the review (unix time)
    * reviewTime - time of the review (raw)
    
* Product Metadata Dataset
    * asin - ID of the product, e.g. 0000031852
    * title - name of the product
    * price - price in US dollars (at time of crawl)
    * imUrl - url of the product image
    * related - related products (also bought, also viewed, bought together, buy after viewing)
    * salesRank - sales rank information
    * brand - brand name
    * categories - list of categories the product belongs to

~~We temporally consider these two datasets, and we are looking for some external dataset that can help us, but these will be discussed later.~~

# Update in milestone2
* Data pre-processing
   * Drop the features we are not interested
   * Select data related to our topic
   * Transform data into proper format
* Data general analysis and specific analysis
   * Review Analysis 
      * Visualize and analyse average rating distribution
      * Visualize and analyse average rating and the number of reviews through years
      * Visualize and analyse percentage of good rating(>=4) and bad rating(<4)
   * Metadata Analysis
      * Analyse 'nan' values distribution or 0-value proportion of each feature
      * Analyse and visualise the distribution of specific features
   * Merge review data and metadata
   
   * Sepecific Analysis
      *  Visualize and analyse rating trend of categories though years
      *  Visualize and analyse the trend of reviews' quantity of different categories through years

   * Correlation Analysis
      * Analyse correlation between reviews' quantity and salesRank
      * Analyse correlation between reviews' quantity and Price
      
# Plan to do in milestone 3
* Give the words in review text part of speech(POS) tags. We plan to select Noun, Adjective, Adverb from review text and calculate the frequency of words by using Spacy library.
* Use Wordcloud library to display the key words in review text.
* Do sentiment analysis on reviews text and get the sentiment of a text. We plan to use nltk library (etc. Vader module) to quantify positiveness and negativeness of review text.
* Use machine learning method to predict the tendency of rating and review quantity. We plan to use to sklearn library or other relevant libraries to realize it.
* The ‘related’ feature of data is not used in Milestone 2, we may consider to explore and analyse further to see whether we could recommend a related product.
* The length of review is also our interested aspect of review, we plan to find the relationship between rating and it.
* Create a well-formed data story or report and create a plan for presentation and poster creation.

# Update in milestone 3
* Give the words in review text part of speech(POS) tags. We display Noun, Verb,  Adjective and Adverb from review text through years .
* we use Wordcloud library to display the key words in review text, such as product, work, far and good for Noun, Verb,  Adjective and Adverb 
* Do sentiment analysis on reviews text and get the sentiment of a text. we normalize the review context by setting a range of the sentiment compound score from [-1,1] to [1,5]
* Use machine learning method to predict the tendency of rating and review quantity. We use sklearn library or other relevant libraries to realize it.
* ~~The ‘related’ feature of data is not used in Milestone 2, we may consider to explore and analyse further to see whether we could recommend a related product.~~
* ~~The length of review is also our interested aspect of review, we plan to find the relationship between rating and it.~~
* Create a well-formed data story or report and create a plan for presentation and poster creation.


# Contributions of group members 
Liang Yueran: Website design, Sentiment Analysis, Metadata Analysis, data story sharing ;   
Luo Yaxiong: Data Story Formulation, Special Day Analysis, Data Pre-proessing, Coming up with the algorithm;  
Xia Shengzhao: Seasonal Decomposition and Rrediction, Key words and Bigrams Analysis, Correlation;  
    
# General Milestone

The schedule of our project:

05/11/2018 - 15/11/2018: Data collection and wrangling

* Access the dataset and fully understand it so that all members can be assigned to their interested parts.

16/11/2018 - 29/11/2018: Data analysis 

* Look at the attributes of dataset and find some proper methods to do a data analysis like distribution, visualization, statistic analysis.

30/11/2018 - 10/12/2018: Review analysis and Data visulization

* Analyse review text and show the visualization in plots

11/12/2018 - 16/12/2018: Conclusion and Report

17/12/2017 - TBD: Poster & Presentation

# Data Reference
R. He, J. McAuley. Modeling the visual evolution of fashion trends with one-class collaborative filtering. WWW, 2016<br/>
J. McAuley, C. Targett, J. Shi, A. van den Hengel. Image-based recommendations on styles and substitutes. SIGIR, 2015
<!-- # Questions for TAa
Add here some questions you have for us, in general or project-specific. -->
