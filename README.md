# Starbucks Project

The dataset provided in this portfolio exercise was originally used as a take-home assignment provided by Starbucks for their job candidates. It consists
of a project involving **A/B tests** and **modeling**.

## Table of contents
1. [Description](#Description)
2. [Installation](#Installation)
3. [File Descriptions](#File_Descriptions)
4. [Licensing, Authors, Acknowledgements](#Licensing-Authors-Acknowledgements)


## Description

**Data** 

The data for this exercise consists of about 120,000 data points split in a 2:1 ratio among training and test files. In the experiment simulated 
by the data, an advertising promotion was tested to see if it would bring more customers to purchase a specific product priced at $10. Since it 
costs the company 0.15 to send out each promotion, it would be best to limit that promotion only to those that are most receptive to the promotion. 
Each data point includes one column indicating whether or not an individual was sent a promotion for the product, and one column indicating whether 
or not that individual eventually purchased that product. Each individual also has seven additional features associated with them, which are provided 
abstractly as V1-V7.

**Objective**

The task is to use the training data to understand what patterns in V1-V7 indicate that a promotion should be provided to a user. Specifically, the 
goal is to maximize the following metrics:

**Incremental Response Rate (IRR)**
IRR depicts how many more customers purchased the product with the promotion, as compared to if they didn't receive the promotion. Mathematically, 
it's the ratio of the number of purchasers in the promotion group to the total number of customers in the purchasers group (treatment) minus the ratio 
of the number of purchasers in the non-promotional group to the total number of customers in the non-promotional group (control).

**Net Incremental Revenue (NIR)**
NIR depicts how much is made (or lost) by sending out the promotion. Mathematically, this is 10 times the total number of purchasers that received the 
promotion minus 0.15 times the number of promotions sent out, minus 10 times the number of purchasers who were not given the promotion.

## Installation

- python version 3.6.5
- There shouldn't be any required downloads in order to run this program

## File_Descriptions

- Starbucks.ipynb: notebook with analysis and decisions made in creating a model used to make predictions
- test_results.py: function to evaluate the model 
- Test.csv: data from real world interaction to test model predictions
- training.csv: data used for the analysis and training of the model

## Licensing-Authors-Acknowledgements

Must give credit to Starbucks for the data. The code can be used as any person demands.
