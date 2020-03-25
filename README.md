# Udacity Data Scientist Nanodegree

### Starbucks Capstone Project



## Table of Contents
1. [Project Motivation](#ProjectMotivation)
2. [Installation](#Installation)
3. [File Descriptions](#File)
4. [Results](#Results)
5. [Licensing and Acknowledgements](#Licensing)

## Project Motivation <a name="ProjectMotivation"></a>

- Once every few days, Starbucks sends out an offer to users of the mobile app. 
An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free).
Some users might not receive any offer during certain weeks.Not all users receive the same offer, and that is the challenge to solve in this project.
- we will combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type.
This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product
whereas Starbucks actually sells dozens of products.
- The problem statement I am aiming to answer are :<br/>
**(1)** Discover customer attributes as Age , income, gender.<br/>
  **(2)** Discover How long did the users become members ? .<br/>
  **(3)** predict whether or not the offer will respond by the person.<br/>
Using the data provided (portfolio, profile, Transactional),I answer first and second question using charts
and i answer the third question using 6 classification models.

## Installation <a name="Installation"></a>

This project requires Python 3.x and Python libraries in `requirements.txt`

## File Descriptions <a name="File"></a>
`Starbucks_Capstone_notebook.ipynb` jupyter notebook<br/>
`Starbucks_Capstone_notebook.html` jupyter notebook HTML <br/>
`requirements.txt` necessary libraries <br/>
`portfolio.json` Offers sent during 30-day test period (10 offers x 6 fields)<br/>
`profile.json` Rewards program users (17000 users x 5 fields)<br/>
`transcript.json` Event log (306648 events x 4 fields)<br/>

## Results <a name="Results"></a>

Actually, most metrics are great and I like to evaluate many metrics but from our business question and since we have a simple classification problem,
 **Accuracy** is a great metric to evaluate my models,
 because We want to see how well our model by seeing the number of correct predictions vs total number of predictions.
 and anwser the question : How many custemrs use Starbucks offers?.this is my opinion and reasoning on why to use the easiest metric (accuracy).

My analysis suggests that the resulting GaussianNB model has an bogo training data accuracy of 64 and bogo test accuracy of 62 .
discount training accuracy of 0.929 and discount test accuracy of 60 suggests that the GaussianNB model I constructed did not overfit the training data.

Blog Post : https://medium.com/@mlataibrahim/analyzing-customer-behavior-on-the-starbucks-rewards-mobile-app-95c60a3217c5?sk=6c4569a8b279de1d6889a1684f263e6a

## Licensing and Acknowledgements <a name="Licensing"></a>

Credits must be given to Udacity for the starter codes and Starbucks for provding the data used by this project.