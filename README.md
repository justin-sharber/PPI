# Analyzing the Predictability of the Poverty Probability Index
The ![Poverty Probability Index / **PPI**](https://www.povertyindex.org/) is a measurement tool for predicting poverty.  This project asks the question of whether the PPI for individuals can be predicted well from general data provided by 


This project predicts the from high-level data about individuals provided by the Finanical Inclusion Insights household surveys.

The best model found was a decision tree regressor.  Predictive accuracy was limited.  Only a low R-squared score of 0.422 was aciheved.  

I investigate this low performance and point to two issues in the data:
1. The target is a continuous variable, but the data provides almost no numerical basis for regression.
2. The features exhibit significant information overlap, limiting the real information content of the predictive basis.

This repository holds the data report, scripts, and data files used for review.  

## Repository Contents
**[Executive Report: Predicting the PPI](PPI_data_report.pdf)** - Full report of the project and findings.

**[Analytical Jupyter Notebook](code/PPI.ipynb)** - Walks through the data analysis, particularly evaluation of the incoming data.  A more informal approach.

**Preparatory Scripts** - Several Python scripts must be run in succession to respect dependencies: *data*, *encode*, and *model*.  In addition, two other supplemental scripts can be run optionally.  

1. data.py
1. explore.py
1. encode.py
1. model.py
1. present.py

## Notes   
- The predictive model was created and hosted in Azure Machine Learning Studio.  That model is not contained here.
