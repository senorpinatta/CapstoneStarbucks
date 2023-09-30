# Introduction

Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. 

Not all users receive the same offer, and that is the challenge to solve with this data set.

In this analysis, we will combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type.

## Problem Statement

This is the final project in Udacity's Data Scientist Nanodegree. The purpose of this project is to use and demonstrate the Software, Date, and ML Engineering techniques learned in this program on specially curated data provided by Starbucks.

The defining questions to be answered in this project are:

**Question 1. Which are the defining features of an effective offer?**

**Question 2. Can these features be used to predict whether an offer will be effective? (binary classification)**

## Project File Structure
- Root
    - Starbucks_Capstone_notebook.ipynb
    - data
        - portfolio.json
        - profile.json
        - transact.json
    - README.md

## Results Summary
  
The 2 main questions of the dataset were:
1. Which are the defining features of an effective offer?

The answer to the first question revealed that the same features had similar impact on whether an offer ended up being effective or not.

**For each offer type, in varying orders `income`, `age`, `years_of_membership` were the most important features.**

2. Can these features be used to predict whether an offer will be effective?

With some refinement, the randomforest models all proved more accurate than the baseline decisiontree model. 

- The refined randomforest bogo model had an accuracy of ~72%

- The refined randomforest discount model had an accuracy of ~70%

- The most accurate model was the refined randomforest informational model with an accuracy of ~80%.

## Blogpost

A blogpost providing further detail into the process of analysis can be found [here](https://seattleairbnbanalysis.wordpress.com/2023/09/30/how-starbucks-can-become-the-king-of-promotional-offers/)

## Libraries Used

- pandas==0.23.3
- numpy==1.19.5
- matplotlib==3.3.4
- scikit-learn==0.19.1
- seaborn==0.8.1

## Acknowledgments

- Starbucks provided dataset.
    - data/[transcript.json, profile.json, portfolio.json]

- Statistical Definitions
    - medium.com/analytics-vidhya/accuracy-vs-f1-score-6258237beca2

- Existing projects used as a reference
    - https://github.com/JcFreya/Starbucks-Capstone-Challenge
    - https://github.com/Sajjadmanal/Udacity-Data-Scientist-Nanodegree/tree/master/Project-6/Capstone_Project

- Mentor Feedback
    - https://knowledge.udacity.com/questions/845663
