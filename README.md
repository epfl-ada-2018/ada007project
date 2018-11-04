# Title
Title: **Analysis on products realatd to health on Amazon**

Team members: Liang Yueran, Luo Yaxiong, Xia Shengzhao

# Abstract
Improving health condition is an indispensable part of society improvement. In this project, we focus on the Amazon product data to draw a conclusion on how to promote health. Our goal is to analyze the popularity of products related to physical health from different points of views, such as providing a visualization of data to show the changing trend of amount of reviews,  comparing average rating of the products. We hope to give people an insight of how these products influence people’s life. Are they becoming more and more important or are they losing the interest of these kinds of products?  Morever, good recommendations are essential to promote these products for people interested in them. By combining rating, sentiment analysis of the review and other useful features of data, we also want to make a reasonable recommendations.

# Research questions

* How to define the popularity of healthy product specifically?

* What's the most popular Healthy product? How the average of rating varies between different categories?

* How the ratings of healthy product change and how people rate for different healthy products?

* what are the keywords in review for several popular healthy products?

* How to combine the serveral features of data to give recommendations (based on the ratings, based on the review) ?


# Dataset

The primary dataset that we would like to use is the [Amazon Review Dataset](http://jmcauley.ucsd.edu/data/amazon/). This dataset includes reviews (ratings, text, helpfulness votes), product metadata (descriptions, category information, price, brand, and image features)

### Category 

We will mainly concern several category listed below:
* Category information
    * Sports and Outdoors
    * Health and Personal Care

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

We temporally consider these two datasets, and we are looking for some external dataset that can help us, but these will be discussed later.

# A list of internal milestones up until project milestone 2

The schedule of our project:

05/11/2018 - 15/11/2018: Data collection and wrangling

Fully understand the dataset and have access to it so that all members can be assigned interested parts.

16/11/2018 - 29/11/2018: Data analysis 

Look at the attributes of dataset and find some proper statidtic methods to hava a data analysis.

30/11/2018 - 06/12/2018: Data story and Data visulization

Creat a interesting and meaningful data story for our analysis and show the visuliztion in plots.

07/12/2018 - 16/12/2018: Conclusion and Reprot

17/12/2017 - TBD: Poster & Presentation

<!-- # Questions for TAa
Add here some questions you have for us, in general or project-specific. -->
