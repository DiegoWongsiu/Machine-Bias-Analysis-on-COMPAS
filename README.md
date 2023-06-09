# Machine-Bias-Analysis-on-COMPAS

## Introduction
Most of the part of this project is a self-implementation of the original analysis conduted by Propublica. The original story and the methodology comes from https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing and https://www.propublica.org/article/how-we-analyzed-the-compas-recidivism-algorithm . In addition, this project explores a cost-sensitive learning technique to help improve the fairness problem.

The analysis are mainly splitted into 3 parts. 
- Basic analysis: This part mainly focus on the analysis of overall situation of the dataset and some of the detailed description on specific features, including charge_degree, legal_status, raw_score, decile_score, recidivist, sex, race, age, r_days_from_arrest, rec_supervision_level. 
- Recidivism Factor analysis: This part contains the analysis of different factors, including personal features such as sex, age, race and marital status, COMPAS assessment result such as decile score of recidivism, charge degree and supervision level.
- Bias(Fairness) Analysis: This notebook focus on the analysis of racial bias of the recidivism scoring predicted by COMPAS, and a cost-sensitive learning method to solve the problem.

## Objective
The objective of this data analysis is to identify the factors that contribute to recidivism among offenders and the biased prediction problem on COMPAS assessment, and propose a cost-sensitive learning to mitigate it. 

## Content

### Basic Analysis
1. Overall situation
2. Detail Description of specific features. (charge degree, legal status, decile score, recidivist, sex, race, age)

### Factor Analysis
1. Correlation of factors.
2. Feature analysis classified by recidivist. 
3. Hypothesis test on the significant factors. 

### Bias Analysis
1. Thresholding the scoring system
2. Racial bias analysis on accuracy, false positive rate, positive predictive rate, false omission rate.
3. Cost sensitive learning

## Result
African-Americans are disadvantaged in terms of false positive rate for 20% comparing with the others. Their cost grows higher than the others as the harm of false positive increases. The cost sensitive learning mitigated the situation.

