# Predicting the PPI
This project predicts the PPI from high-level data about individuals provided by the Finanical Inclusion Insights household surveys.

Predictive accuracy was limited.  The project's metric is the R2 score.  Only a low R2 score of 0.422 was aciheved.  

I investigate this low performance and point to two issues in the data:
1. The target is a continuous variable, but the data provides almost no numerical basis for regression.
2. The features exhibit significant information overlap, limiting the .

This repository holds the data report, scripts, and data files used for review.  All the analysis appears in the data report **["Predicting the PPI."](PPI_data_report.pdf)**

See the project notebook here: 
**[companion Jupyter notebook](code/PPI.ipynb)**

* [Alternate link at NBViewer](https://nbviewer.jupyter.org/github/JShibby/PPI/blob/master/code/PPI.ipynb)

## Preparatory Scripts
Several Python scripts must be run in succession to respect dependencies: *data*, *encode*, and *model*.  In addition, two other supplemental scripts can be run optionally.  Numbers show necessary scripts; bullets show the optional scripts.  

1. data.py
1. explore.py
1. encode.py
1. model.py
1. present.py
   
The predictive model was created and hosted in Azure Machine Learning Studio.
