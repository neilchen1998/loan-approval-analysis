# Analyzing Important Factors in the Loan Approval Process


## Overview

This project looks into the factors that hold the most weight when an applicant’s loan is approved or denied within
the state of California. The motivation for this is to provide more transparency regarding the loan approval process, especially in
a time where more and more Californians are looking towards taking out loans to afford buying a home. The data set used in
this project is taken from the Consumer Financial Protection Bureau. Factors such as the applicant’s race, income, locale,
and sex are analyzed. Both decision tree and k-means clustering machine learning models are used to predict whether given loan
applications are approved or denied.

## Dataset [1]

The data set used in this project comes from the Consumer
Financial Protection Bureau. This data is collected under the
Home Mortgage Disclosure Act (HMDA) and contains information
regarding individual loan applications [1]. In particular,
the data set for this project only contains information on
mortgages for single family homes filed in 2017 within the
state of California.

## Data Analysis

We plotted the approval versus denial ratio for
each given race in the figure below. For each race, the rates of
approved loans versus denied loans are relatively equivalent
in value. This leads to the conclusion that there is no racial
bias when determining loan approval or denial.

<picture>
  <img src="https://github.com/neilchen1998/loan-approval-analysis/blob/main/graphs/approval-vs-denial-rate-by-race.png" width="250" height="300"/>
</picture>

## Approaches

* Decision Tree Model

Decision tree machine learning models are non-parametric
supervised models used for regression and classification problems.
Our goal is to create a model that can predict whether a
loan is approved or denied by learning simple decision rules
inferred from the training data features. This model is able
to handle both numeric variables (the income of the applicant
and the loan amount) and categorical variables (the sex, the
race, and the county of the applicant). Furthermore, it uses
a white box model, hence we can visualize it and it can be
explained easier than a black box model such as the ones used
in artificial neural networks.

* K-Means Model

K-means machine learning models are unsupervised models,
meaning that the training data that goes in to the model is
not labeled. Essentially, the model does not know in our case
which data values constitute approved loans, and which are
denied loan applications. The model must figure out on its
own how to distinguish approved loans from denied loans.
Upon initializing the k-means algorithm, we determine a set
number of centroids to cluster our data around, In our case, we
use two centroids for approved and denied loan applications.

## Results

<!-- * Naive Bayes

<picture>
  <img src="https://github.com/neilchen1998/image-segmentation-project/blob/main/results/naive-bayes-result.jpg" width="250" height="250">
</picture> -->

## Authors

* [Neil Chen](pychen@ucsd.edu)
* [Callie Hartzog](chartzog@ucsd.edu)

## Reference

1. [Home Mortgage Disclosure Act (HMDA)](https://www.consumerfinance.gov/data-research/hmda/historic-data/)
